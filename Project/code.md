import time
from colorama import Fore


def try_signup(name: str, password: str) -> bool:
    with open('/Users/edvards/PycharmProjects/unit1/project1/users2.csv', mode='a') as file:
        file.writelines(f'{name},{password},0\n')  # Writing a line with a newline character at the end
        print('account created')
        file.close()


def try_login(name: str, password: int) -> bool:
    with open('/Users/edvards/PycharmProjects/unit1/project1/users2.csv', mode='r') as file:
        content = file.readlines()
        file.close()

    success = False

    for line in content:
        uname = line.split(',')[0]
        upass = line.split(',')[1].strip()  # strip() removes \n
        if uname == name and upass == password:
            success = True
            print('login data recognized')
            break

    return success

def balance_check():
    with open('/Users/edvards/PycharmProjects/unit1/classes/atm.csv', mode='r') as f:
        data = f.readlines()
    balance = 0
    for line in data:
        date, amount = line.strip().split(',')
        line = f'{date}, {amount}\n'
        balance += int(amount)
    return balance

answer = input('Would you like to sign in or register: type s or r: ')
while answer != 's' and answer != 'r':
    answer = input('Error, indicate if you would like to sign in or register: type s or r ')

if answer in "s":
    attempts = 3
    in_name = input("Enter your username: ")
    in_pass = input("Enter your password: ")
    result = try_login(name=in_name, password=in_pass)
    attempts -= 1
    while not result and result == False and attempts > 1:
        in_name = input(Fore.RED + "[Error, try again] Enter your username: ")
        in_pass = input("Enter your password: ")
        result = try_login(name=in_name, password=in_pass)
        attempts -= 1
    if attempts == 0:
        print(Fore.RED + 'exiting...')
        exit(1)  # 1 is the code for exit without errors

elif answer in 'r':
    sign_name = input('Create a username of your choice: ')
    sign_pass = input('Create a password of your choice: ')
    try_signup(name=sign_name, password=sign_pass)

# the program continues here if it doesn't close
time.sleep(1)
print(Fore.RED + "Loading...")
time.sleep(1)
print(Fore.RED + 'Acess granted')
# the rest of the program

import datetime
from colorama import Fore

from classes.my_lib import print_menu, validate_int

def menu():
    print(Fore.GREEN + '\nPlease choose an option' + Fore.RESET)

    menu_1 = ["Deposit", "Withdraw", "Balance", "Graph", "Suggestion", "Exit"]
    print("The menu is:")
    print_menu(menu_1)

    option = -1 #this could be any value but 1 2 3
    while option not in [1, 2, 3, 4, 5, 6]:
        option = validate_int(msg="Plesase enter an option: ", menu = menu)

    if option == 4:
        with open('/Users/edvards/PycharmProjects/unit1/classes/atm.csv', mode ='r')as f:
            data = f.readlines()
        deposits = 0
        withdraws = 0
        for line in data:
            date, amount = line.strip().split(',')
            if int(amount)>0:
                deposits+= int(amount)
            else:
                withdraws += -1*int(amount)
        #create a simple graph
        deposits = deposits // 100 #integer division
        withdraws = withdraws // 100
        bar_deposits = "deposits".ljust(20)
        bar_withdraws = "withdraws".ljust(20)
        bar_balance = "balance".ljust(20)

        balance = balance_check()
        for x in range(deposits):
            bar_deposits += '▥'
        for x in range (withdraws):
            bar_withdraws += '▥'
        for x in range(balance//10):
            bar_balance += '▥'
        print(f'{bar_deposits} {deposits}')
        print(f'{bar_withdraws} {withdraws}')
        print(f'{bar_balance} {balance}')
        menu()
    if option == 1: #deposit
        amount = validate_int(msg="Please enter amount to deposit: ", menu="")
        date = datetime.date.today() # today's date
        line = f'{date},{amount}\n'
        with open('/Users/edvards/PycharmProjects/unit1/classes/atm.csv', mode ='a') as f:
            f.writelines(line)
        print('saved')
        balance = balance_check()
        today = datetime.date.today()
        print(f"Your balance {today} is $ {balance}")
        menu()

    if option == 3: #calculate balance
        balance = balance_check()
        today = datetime.date.today()
        msg = f"Your balance {today} is $ {balance}"
        print(msg)
        menu()

    if option == 5: #coin worth, suggestions
        from bs4 import BeautifulSoup
        import requests

        def check_last() -> float:
            with open('/Users/edvards/PycharmProjects/unit1/project1/doge_value.csv', mode='r') as doge_value:
                value = doge_value.readlines()
                print(f"{value[0]} fetched from the database")
                return value[0].split('\n')[0]


        def add_new(value):
            with open('/Users/edvards/PycharmProjects/unit1/project1/doge_value.csv', mode='w') as doge_value:
                doge_value.writelines(f"{value}")
                print(f"{value} added to the database")


        url = 'https://crypto.com/price/dogecoin'
        page = requests.get(url)
        soup = BeautifulSoup(page.text, 'html5lib')
        output = soup.find('span', class_="chakra-text css-13hqrwd").text.strip('$ USD')
        output = float(output)
        last_value = float(check_last())
        difference = output - last_value
        add_new(output)
        print(f"Difference between now and last value: {round(difference, 4)}")
        if difference < 0:
            print('I advise you to buy since it dropped in value and future profit is possible')
        elif difference > 0:
            print('I advise you to sell since it rose in value and profit is possible')
        else:
            print('The value has stayed the same, wait')

        menu()

    if option == 2:
        amount1 = validate_int(msg="Please enter amount to withdraw: ", menu="")
        date = datetime.date.today()  # today's date
        balance = balance_check()
        if balance - amount1 >= 0:
            line = f'{date},{amount1*-1}\n'
            with open('/Users/edvards/PycharmProjects/unit1/classes/atm.csv', mode='a') as f:
                f.writelines(line)
            print(f'{amount1} has been withdrawn from your account')
            print(f'your balance is {balance-amount1}')
        else:
            print('You do not have enough money in your account, call your dad')
        menu()

    if option == 6:
        exit('See you soon!')

menu()
