# Crypto Wallet

![image](https://github.com/Rokyyz/unit-1CS/assets/134658259/463192b5-ed8c-454a-9407-dcdb0f2bf38e)
[1]

# Criteria A: Planning

## Problem definition

Ms. Sato is a local trader who is interested in the emerging market of cryptocurrencies. She has started to buy and sell electronic currencies, however, at the moment she is tracking all his transactions using a ledger in a spreadsheet which is starting to become burdensome and too disorganized. It is also difficult for Ms. Sato to find past transactions or important statistics about the currency. Ms Sato is in need of a digital ledger that helps her track the amount of the cryptocurrency, and the transactions, along with useful statistics. Ms. Sato is currently interested in the cryptocurrency DogeCoin and wishes to use it as her main cryptocurrency in the digital ledger.

Apart from these requirements, Ms. Sato is open to exploring a cryptocurrency selected by the developer.

An example of the data stored is 

| Date | Description | Category | Amount  |
|------|-------------|----------|---------|
| Sep 23 2022 | bought a house | Expenses | 10 BTC |
| Sep 24 2022 | food for house celebration | Food | 0.000001 BTC |


## Proposed Solution
Design statement:
I will design and make an electronic ledger for a client, Ms. Sato, a cryptocurrency trader keen on learning more skills surrounding trading cryptocurrencies. The electronic ledger will track cryptocurrency transactions in the account, display the current value of the chosen crypto coin, compare it to a previous data point, and make suggestions regarding investment opportunities using the software Python (1). The client likes for her data to remain safe so I will try to introduce a login and registration system (2). Ms. Sato also fancies her account data regarding all withdraws, deposits and overall balance to be displayed in an easy-to-read way, so I decided to try and implement these data values in a graph (3). It will take approximately 2-3 weeks to make and will be evaluated according to the criteria shown in the success criteria, including functionality, and usability.

## Description of coin 

"Dogecoin is an open-source, dog-themed cryptocurrency established in 2013 by Jackson Palmer and Billy Markus. It's based on an internet meme. Dogecoin features a Shiba Inu, a Japanese breed of dog, as its logo. It is based on Litecoin and uses the same proof-of-work technology. The currency’s faceplate features the Shiba Inu’s head with the letter “D” superimposed. Although the value of an individual Dogecoin is very small (often a portion of a cent) the massive number of Dogecoins in circulation correlates to a market capitalization of over $1 billion." [2,3]


## Justification of the tools/structure of your solution

Why Dogecoin:

* Inflationary Supply:
Unlike Bitcoin, which has a capped supply, Dogecoin has an inflationary supply model with a soft cap of 5 billion coins per year. While this may seem counterintuitive, it could contribute to a more stable and predictable issuance, potentially influencing its long-term viability as a medium of exchange.

* Low Transaction Costs:
Dogecoin has historically had low transaction fees compared to some other cryptocurrencies, making it an attractive option for microtransactions and everyday use. Its low fees make it appealing for certain types of transactions, and this utility can affect its long-term value.

* Integration in Payment Systems:
Dogecoin has been integrated into various payment systems and platforms, enabling users to use it for online transactions and tipping. Analyzing its adoption in real-world applications and partnerships can provide insights into its potential for mainstream acceptance.


Why Python:

* Interface
Python has a friendly and easy-to-understand interface thus making it easy to both code and work in the terminal and run/test the code.
It has multiple built-in libraries and toolkits thus making it easier and more time efficient to code. All of this helps Ms. Sato to easily overview and work in the electronic ledger.

* Flexibility and multifunction
Python offers great flexibility in terms of code, input, and imported items thus assuring multifunctional features allowing for unique features like in-time updates on a certain item. In Ms. Sato's case, it helps her to monitor the value of the coin and advise her on what to do with her portfolio.

* Maintainance and readability
Because Python is so flexible with multiple functions and because it makes all of these possibilities to be coded in a simple manner with easy-to-understand, clean, and easy syntax software updates and maintenance are easy to manage and there is way lower risk for a bug to appear in the code. This assures that this software will be useful to Ms. Sato for a long time, will run without problems, and can be easily updated and further developed.

* It is the most popular and widely used programming language and it is also among the fastest-growing programming languages in the tech industry [4]. According to CodingNomads, 30% of developers wish to learn Python the most [5]. As a result of the language's popularity, the program is easier for many developers to understand than languages like C or Javascript. This will benefit the digital ledger because it makes it simple for new programmers to understand and easily interact with the code and advance its development. There are also a wide range of libraries that are available in Python which can be easily accessed using a basic syntax [6]. Further, Python is a very efficient language that does not require the programmer to compile their program before executing it. Due to the fact that programmers do not have to invoke a compiler and run the compiler that helps turn source files into compiled class files, they can just simply run a ".py" file [7].


## Success Criteria


1. The electronic ledger is a text-based software (Runs in the Terminal).
2. The electronic ledger displays the selected cryptocurrency's description including year of release, creator, basic description, inspiration behind creation, and worth.
3. The electronic ledger allows to enter, withdraw, and record transactions.
4. The electronic ledger advises whether to buy or sell the coin, based on the record of transactions. (Issue tackled(1))
5. The electronic ledger has a login and registration interface. (Issue tackled(2))
6. The electronic ledger graphs your portfolio value and the history of your transactions. (Issue tackled(3))

# Criteria B: Design

## System Diagram

![CommSci](https://github.com/Rokyyz/unit-1CS/assets/134658259/a85865ac-47e9-48db-b8f7-35016ae7cfe5)


**Figure 1.** This is a system diagram, it starts with the input - the keyboard and it finishes with the output which is the terminal in Pycharm. The computer that is used to program this wallet is a MacBook Air Retina, 13-inch 2018 (the specs are further listed in the diagram) with macOS Ventura Version 13.5.2. The code is coded in Pycharm 3.9.6.

## Flow Diagrams

![Com Sci](https://github.com/Rokyyz/unit-1CS/assets/134658259/a7735c18-e1d9-4323-a579-f41fc46fbd30)

**Fig. 2** This flow diagram illustrates the code calculation for the total balance the user has in their account depending on their deposit and withdrawal history. The code will open, read and append in the"atm.csv" file to see the data inside, and then calculate the difference to find the current balance and converted amount (USD).


![Com Sci 2](https://github.com/Rokyyz/unit-1CS/assets/134658259/3b0c992d-fb24-45fb-8da4-edae60eb649f)

**Fig. 3** This flow diagram displays a 3-bar graph that includes the amount of balance in the user account and the withdraws and deposits made into the account. It calculates the total amount of money deposited, withdrawn and depending on these two variables also the balance and displays it in the same ratio in an organized, categorized bar graph.

![Com Sci 3](https://github.com/Rokyyz/unit-1CS/assets/134658259/61f4ea62-b912-4c10-b511-0a4d7bdfa3fe)

**Fig. 4** 
This flow diagram displays the login and register function when first starting the code. It first asks for the user to indicate whether the user wants to sign in to an already existing account with an allocated password or create a new account with a new password. The new account username with the newly assigned password gets uploaded into the "users2.csv" file. Before logging in after both registering and signing in the code checks if the username and the password pair appear in the "users2.csv" file, if it does then the user gets directed to the next page - the menu, if the pair doesn't match, an error appears.


## Test plan

| Test NO | Type of test        | Area tested                                                                                    | Outcome of test                                                                                                                                                                                                                           | Time estimate | Target completion date | Criterion |
|---------|---------------------|------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Unit testing        | Advice on whether to buy or sell the coin, based on the coin value and the shift of the value. | Confirm that the program can fetch live data from the internet regarding the value of the coin, put that data into a csv file and then compare the current value with the value of the coin from a previous log in with the help of a csv | 10min         | Sep 18                 | B         |
| 2       | Unit testing        | Login and registration system                                                                  | Confirm that the user is able to sign in with the existing username and password pair that is saved in a csv file. Confirm that the user can create a new account with a new username and password                                        | 10min         | Sep 19                 | B         |
| 3       | Unit testing        | Graph of the portfolio value and the history of transactions.                                  | Confirm that the user can enter/withdraw and check the account balance as well as that the data can be graphed and displayed.                                                                                                             | 10min         | Sep 19                 | B         |
| 4       | Unit testing        | Login and sign up csv files                                                                    | Confirm that the data is stored correctly, "users2.csv" file can be read and appended thus also making sure that the program can check for correct account data. Confirm that the username is unique.                                     | 15min         | Sep 20                 | B         |
| 5       | Unit testing        | Balance check                                                                                  | Confirm that the balance is calculated correctly and then added to the "atm.csv" file and can be later displayed to the client on demand.                                                                                                 | 15min         | Sep 20                 | B         |
| 6       | Unit testing        | Menu check                                                                                     | Confirm that the menu has all the needed options and they can be interacted with, when demanded the code takes the user to the chosen menu option.                                                                                        | 15min         | Sep 20                 | B         |
| 7       | Unit testing        | Data fetch                                                                                     | Confirm that the code updates frequently and fetches the correct numbers and ads to the "doge_value.csv" file.                                                                                                                            | 15min         | Sep 23                 | B         |
| 8       | Integration testing | Login and registration system                                                                  | Confirm that the registration and login functions work well with one another.                                                                                                                                                             | 10min         | Sep 24                 | B         |
| 9       | Integration testing | Data fecth                                                                                     | Confirm that the data fetch functions work well with one another.                                                                                                                                                                         | 10min         | Sep 26                 | B         |
| 10      | System testing      | General                                                                                        | Confirm that the system flows smoothly with the use of the menu option.                                                                                                                                                                   | 15min         | Sep 26                 | B         |
| 11      | Userbility Testing  | General                                                                                        | Confirm that the system is friendly and easy to understand for the users                                                                                                                                                                  | 15min         | Sep 29                 | B         |

## Records of Tasks

| Task No | Planned Action                                                                                                            | Planned Outcome                                                                                                                                                                                                                                                                                                                                                                                   | Time estimate | Target completion date | Criterion |
|---------|---------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Meeting with the client                                                                                                   | Talk with the client to discuss their needs and what they expect from the program as well as think of solutions to the problem                                                                                                                                                                                                                                                                    | 10min         | Sep 13                 | A         |
| 2       | Come up with the problem definition                                                                                       | Write a clear problem definition on GitHub                                                                                                                                                                                                                                                                                                                                                        | 15min         | Sep 13                 | A         |
| 3       | Come to an agreement with the client regarding the success criteria                                                       | Write a clear list of the success criteria for a measurable outcome and that the problem is resolved                                                                                                                                                                                                                                                                                              | 10min         | Sep 13                 | A         |
| 4       | Come up with a proposed solution for the client                                                                           | Write a solution on how to deal with the problem given by the product that suits both the client and developer                                                                                                                                                                                                                                                                                    | 15min         | Sep 13                 | A         |
| 5       | Create system diagram                                                                                                     | To have a clear idea of the hardware and software requirements for the proposed solution                                                                                                                                                                                                                                                                                                          | 10min         | Sep 13                 | B         |
| 6       | Create a login system                                                                                                     | To have a flow diagram and the code for the login system                                                                                                                                                                                                                                                                                                                                          | 30min         | Sep 14                 | B, C      |
| 7       | Create the menu options with "Deposit", "Withdraw", "Balance", "Graph"                                                    | When login or signup is complete the client is met with the main menu where the client can choose between the 4 mentioned options                                                                                                                                                                                                                                                                 | 120min        | Sep 19                 | C         |
| 8       | Create a code that takes live data of DogeCoin value from internet and updates it with each login along with a suggestion | When selecting an option "Suggestion" in the main menu the client can see the current value of the coin as well as the value of the coin at the previous log in. These 2 values are compared and based on the result a business suggestion on whether to buy or sell the cryptocoin.                                                                                                              | 90min         | Sep 21                 | C         |
| 9       | Add "Suggestion", "Description" and "Exit" options to the menu                                                            | Adding 3 new options to the menu code, "Suggestion", "Description" and "Exit". "Suggestion" has the values of the coin as well as the business advice, "Description" includes the selected cryptocurrency's description including year of release, creator, basic description, inspiration behind creation, and worth. "Exit" offers an easy way to finish your actions in the electronic ledger. | 60min         | Sep 23                 | C         |
| 10      | Add a signup system to login                                                                                              | An offer is made to the client to either create an account along with a password or if the client's account with a set password already exists, log in to the account. The account details are registered and stored in a csv file.                                                                                                                                                               | 45min         | Sep 27                 | C         |
| 11      | Add an option to continue after the actions in another menu option is done                                                | After the client has completed the intended action within a menu option, the code offers to go to another menu option instead of exiting the code.                                                                                                                                                                                                                                                | 15min         | Sep 27                 | C         |
| 12      | Meet up with client to show progress and get feedback                                                                     | Show the client the progress with the code to gather the satisfaction result and listen to possible improvements that the client wants to be made                                                                                                                                                                                                                                                 | 25min         | Sep 29                 | A, B, C   |
| 13      | Write the description of the coin and citations                                                                           | Write the selected cryptocurrency's description including year of release, creator, basic description, inspiration behind creation, and worth in the success criteria.                                                                                                                                                                                                                            | 10min         | Oct 3                  | A         |
| 14      | Write the justification of the tools/structure of your solution and tools used                                            | Write the justification for the choice of crypto coin, code language, and tools used while coding.                                                                                                                                                                                                                                                                                                | 30min         | Oct 3                  | A, C      |
| 15      | Create flow charts for the code along with a description                                                                  | Draw flowcharts on important and difficult parts of the code and upload the image along with a description to GitHub.                                                                                                                                                                                                                                                                             | 120min        | Oct 4                  | B         |
| 16      | Write description for important code fragments                                                                            | Write the description of basic but the most important lines of code for others to understand it                                                                                                                                                                                                                                                                                                   | 60min         | Oct 4                  | C         |
| 17      | Write test plan                                                                                                           | On GitHub, record the procedures of steps a developer should take to test a program and the expected outcome of each test                                                                                                                                                                                                                                                                         | 60min         | Oct 4                  | B         |
| 18      | Write record of tasks                                                                                                     | On GitHub, record the procedures of steps a developer should take in order to successfully and in time complete a similar project in terms of time or idea.                                                                                                                                                                                                                                       | 60min         | Oct 4                  | B         |
| 19      | Add colour to code                                                                                                        | The interface becomes more pleasing to the eye and more understandable                                                                                                                                                                                                                                                                                                                            | 30min         | Oct 5                  | C         |

# Criteria C: Development

## Techniques used

1. Functions
2. For/while loops
3. Input Validation
4. If/else/elif statements
5. Importation of libraries and csv files
6. List comprehension

## Registration system
My client requires a system to protect private data. I thought about using a login system to accomplish this requirement using an if condition and the open command to work with a csv file.

As you can see in the flow diagram in **Fig 4**, in the first line I am defining a function called try_signup, this function has two inputs of type string, and the output is a boolean representing True if the user logs in correctly or false otherwise. This is saved in the variable success. The next line opens a "users2.csv" file in which the code appends a name and a password pair when the user is trying to create an account, if it is done successfully feedback is given back to the user. The next function try_login has almost the same code as the try_signup function with the only difference being the mode of the csv file - read. This means that the code reads inside the file the 2 arguments. Next up is the for-loop prepares the name and password to be evaluated, compared, and defined further in the code. Further up we can see an if statement which works in the sense if the user chooses the log-in feature and correctly inputs the name and password pair that had already been registered in the csv file, success turns True and the program gives positive feedback to the user. Next, the answer is defined so that when opening the program the client receives the question of whether they would like to sign up or log in. The while loop makes sure either s or r is input, if not it returns negative feedback. If the user has responded with a sign the program keeps checking if the input username and password pair exists in the csv file. If not one attempt out of 3 is subtracted, and the user gets asked again for the correct username and password pair, and if there are no more attempts left the user gets exited out of the program as a safety precaution. If the user chose to register, the program offers just that and appends the new information value pair to the file.

```.py

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

```
## Menu options

My client requires a menu options page in order to easily view and choose the correct action that needs to be done with the portfolio. I thought about creating a function for a menu and then defining a menu with values and then using the print command to accomplish this requirement.

The first line indicates that a function for the menu has been created later in the code recall it easily and/or input data that is needed to be displayed when the function is called/printed. After that, the print statement asks the user to choose an option that is presented below. Later on, the menu items have been actually written down. The other 2 print lines just print what are the options

```.py

def menu():
    print(Fore.GREEN + '\nPlease choose an option' + Fore.RESET)

    menu_1 = ["Deposit", "Withdraw", "Balance", "Graph", "Suggestion", "Description", "Exit"]
    print("The menu is:")
    print_menu(menu_1)

```
## Description of a coin

My client has requested for the electronic ledger to include a basic description of the crypto coin of her choice DogeCoin. I included  the g year of release, creator, inspiration behind creation, and value. I thought about simply printing some relevant information found on the internet regarding the coin.

In the first line, it makes the code check if the user has chosen option 6 which is "Description". If this proves to be right then the following print lines of text are shown on screen.

```.py
    if option == 6:
        print('Dogecoin is an open-source cryptocurrency established in 2013 by Jackson Palmer and Billy Markus\n')
        print("It's based on an internet meme.\n")
        print('Dogecoin features a Shiba Inu, a Japanese breed of dog, as its logo.\n')
        print('It is based on Litecoin and uses the same proof-of-work technology.\n')
        print("The currency’s faceplate features the Shiba Inu’s head with the letter “D” superimposed.\n")
        print('Although the value of an individual Dogecoin is very small (often a portion of a cent)\n')
        print('the massive number of Dogecoins in circulation correlates to a market capitalization of over $1 billion.')

```

## Fetching data, suggestion/advice

My client has requested that I include a menu option where she can view the current value of the coin and how it has changed since the last login to the site. And since she is just starting out as a crypto trader she would like some advice on when to potentially sell or buy the coin. I thought about finding an internet site and fetching live data by inspecting the code that constantly updates the value of the coin. I researched about this on the internet to find the simplest and most easy-to-understand code. I achieved this by creating a function for a new value and then using the open method to write to the doge_value csv file. 

The first line as mentioned opens up a function to later call and input data. After that, the open code writes lines in the doge_value csv file which will fixate the value of the price of the coin after a login has been registered. When it has written these lines, the print statement makes sure that the user sees that the new value of the coin has been added to the csv file. The next line of code defines a variable 'URL' with the web address of Dogecoin's price on crypto.com. Then it sends a GET request to the provided URL and stores the response in the 'page' variable. The line which defines soup creates a BeautifulSoup object, 'soup', to parse the HTML content of the 'page'. Output extracts the text content of a specific HTML element using its class and then converts the extracted text to a floating-point number. The last value calls the function 'check_last()' to retrieve the last stored value and converts it to a float. In order to give the advice the code has to know whether the coin has risen or fallen in value by comparing the current updated value of the coin vs the value of the coin from a previous request. The calling of the function adds the current value to the database. The print message informs the user about the difference between the current and last values, rounded to four decimal places. And the rest of the code evaluates if the difference is positive or negative and depending on the result gives a suggestion .

```.py
        def add_new(value):
            with open('/Users/edvards/PycharmProjects/unit1/project1/doge_value.csv', mode='w') as doge_value:
                doge_value.writelines(f"{value}")
                print(f"$ {value} added to the database")


        url = 'https://crypto.com/price/dogecoin'
        page = requests.get(url)
        soup = BeautifulSoup(page.text, 'html5lib')
        output = soup.find('span', class_="chakra-text css-13hqrwd").text.strip('$ USD')
        output = float(output)
        last_value = float(check_last())
        difference = output - last_value
        add_new(output)
        print(f"Difference between now and last value: ${round(difference, 4)} ")
        if difference < 0:
            print('I advise you to buy since it dropped in value and future profit is possible')
        elif difference > 0:
            print('I advise you to sell since it rose in value and profit is possible')
        else:
            print('The value has stayed the same, wait')

```
## Deposits

My client required an option to deposit her money in her account after the crypto investments that she had made. I thought about creating an input for the client to input the amount of money they had made and wanted to store and then register that amount of money to a database csv file to keep track of the account's transactions.

The first line makes sure that the user has truly chosen to deposit money into the account. The next line asks for the amount of money the user wishes to deposit.  After that with the with open tool, a csv file gets opened and set into the append mode to add lines to the file. It needs to append information on the amount of value that has been deposited to keep track of the account transactions. After the data has been successfully stored, it returns positive feedback back to the user. And with the import function, it sates for today to always be the current date that the login has been made. After everything has been done it prints out the balance in the account so the user can be sure the money has been successfully deposited.
```.py
    if option == 1: #deposit
        amount = validate_int(msg="Please enter amount to deposit: ", menu="")
        line = f'{date},{amount}\n'
        with open('/Users/edvards/PycharmProjects/unit1/classes/atm.csv', mode ='a') as f:
            f.writelines(line)
        print('saved')
        balance = balance_check()
        today = datetime.date.today()
        print(f"Your balance {today} is $ {balance}")
        menu()

```

## Withdraws

My client required an option to withdraw the money she made from trading DogeCoin so she could spend it for her own needs. I thought about creating an input for the client to input the amount of money they wanted to cash out and then register that that amount of money has been taken out of the account to a database csv file to keep track of the account's transactions.

The first line makes sure that the user has truly chosen to deposit money into the account. The next line asks for the amount of money the user wishes to withdraw. And with the import function, it states for the date to always be the current date that the login has been made. After that with the with open tool, a csv file gets opened and set into the append mode to add lines to the file. It needs to append information on the amount of value that has been withdrawn to keep track of the account transactions. However, if the user doesn't have enough money in the account to withdraw the wanted amount, it returns an error and informs the user about the issue. After the data has been successfully stored, it returns positive feedback back to the user. After everything has been done it prints out the balance in the account so the user can be sure the money has been successfully deposited. 

```.py
    if option == 2:
        amount1 = validate_int(msg="Please enter amount to withdraw: ", menu="")
        date = datetime.date.today()  # today's date
        balance = balance_check()
        if balance - amount1 >= 0:
            line = f'{date},{amount1*-1}\n'
            with open('/Users/edvards/PycharmProjects/unit1/classes/atm.csv', mode='a') as f:
                f.writelines(line)
            print(f'$ {amount1} has been withdrawn from your account')
            print(f'your balance is $ {balance-amount1}')
        else:
            print('You do not have enough money in your account, call your dad')
        menu()

```
# Citations

## Works Cited

DataFlair. “Advantages and Disadvantages of Python - How it is dominating Programming World.” DataFlair, 2023, https://data-flair.training/blogs/advantages-and-disadvantages-of-python/. Accessed 5 October 2023. 
[6]

Desmond, Kim, and Caden MacKenzie. “Why Learn Python? 6 Reasons Why it's So Hot Right Now.” CodingNomads, 7 April 2023, https://codingnomads.co/why-learn-python/. Accessed 5 October 2023.
[5]

FRANKENFIELD, JAKE. “Cryptocurrency Dogecoin (DOGE): What It Is, History, and Uses.” INVESTOPEDIA, 9 september 2022, https://www.investopedia.com/terms/d/dogecoin.asp#:~:text=Dogecoin%20is%20an%20open%2Dsource,proof%2Dof%2Dwork%20technology. Accessed 4 october 2023.
[2]

IndustryTrends. “Could Dogecoin (DOGE) Beat Shiba Inu (SHIB) for Good? Analysts Recommend Collateral Network (COLT) to Surpass Both in 2023.” Analytics Insight, 31 May 2023, https://www.analyticsinsight.net/could-dogecoin-doge-beat-shiba-inu-shib-for-good-analysts-recommend-collateral-network-colt-to-surpass-both-in-2023/. Accessed 5 October 2023.
[1]

Rouse, Margaret. “Dogecoin.” Techopedia, 4 September 2023, https://www.techopedia.com/definition/33147/dogecoin#:~:text=Dogecoin%20is%20a%20dog%2Dthemed,capitalization%20of%20over%20%241%20billion. Accessed 4 October 2023.
[3]

Sanyal, Sayantani. “10 Reasons Why Python is One of the Best Programming Languages.” Analytics Insight, 18 February 2022, https://www.analyticsinsight.net/10-reasons-why-python-is-one-of-the-best-programming-languages/. Accessed 5 October 2023.
Vilmate. “Advantages of the Python Language over Other Ones | Vilmate.” VILMATE, 2019, https://vilmate.com/blog/python-vs-other-programming-languages/. Accessed 5 October 2023.
[4]

Vilmate. “Advantages of the Python Language over Other Ones | Vilmate.” VILMATE, 2019, https://vilmate.com/blog/python-vs-other-programming-languages/. Accessed 5 October 2023.
[7]

