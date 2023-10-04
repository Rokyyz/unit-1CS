# Crypto Wallet

# Criteria A: Planning

## Problem definition

Ms. Sato is a local trader who is interested in the emerging market of cryptocurrencies. She has started to buy and sell electronic currencies, however at the moment she is tracking all his transaction using a ledger in a spreadsheet which is starting to become burdensome and too disorganized. It is also difficult for Ms Sato to find past transactions or important statistics about the currency. Ms Sato is in need of a digital ledger that helps her track the amount of the cryptocurrency, the transactions, along with useful statistics. 

Apart for this requirements, Ms Sato is open to explore a cryptocurrency selected by the developer.

An example of the data stored is 

| Date | Description | Category | Amount  |
|------|-------------|----------|---------|
| Sep 23 2022 | bought a house | Expenses | 10 BTC |
| Sep 24 2022 | food for house celebration | Food | 0.000001 BTC |


## Proposed Solution
Design statement:
I will design and make an electronic ledger for a client, Ms. Sato, a cryptocurrency trader keen on learning more skills surrounding trading cryptocurrencies. The electronic ledger will track cryptocurrency transactions in the account, display the current value of the chosen crypto coin, compare it to a previous data point, and make suggestions regarding investment opportunities using the software Python. It will take approximately one 3-4 weeks to make and will be evaluated according to the criteria shown in the success criteria, including functionality, and usability.

## Description of coin and citation

"Dogecoin is an open-source, dog-themed cryptocurrency established in 2013 by Jackson Palmer and Billy Markus. It's based on an internet meme. Dogecoin features a Shiba Inu, a Japanese breed of dog, as its logo. It is based on Litecoin and uses the same proof-of-work technology. The currency’s faceplate features the Shiba Inu’s head with the letter “D” superimposed. Although the value of an individual Dogecoin is very small (often a portion of a cent) the massive number of Dogecoins in circulation correlates to a market capitalization of over $1 billion." [REF1]

[REF1]

Works Cited
FRANKENFIELD, JAKE. “Cryptocurrency Dogecoin (DOGE): What It Is, History, and Uses.” INVESTOPEDIA, 9 September 2022, https://www.investopedia.com/terms/d/dogecoin.asp#:~:text=Dogecoin%20is%20an%20open%2Dsource,proof%2Dof%2Dwork%20technology. Accessed 4 October 2023.
Rouse, Margaret. “Dogecoin.” Techopedia, 4 September 2023, https://www.techopedia.com/definition/33147/dogecoin#:~:text=Dogecoin%20is%20a%20dog%2Dthemed,capitalization%20of%20over%20%241%20billion. Accessed 4 October 2023.

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


## Success Criteria


1. The electronic ledger is a text-based software (Runs in the Terminal).
2. The electronic ledger displays the selected cryptocurrency's description including year of release, creator, basic description, inspiration behind creation, and worth.
3. The electronic ledger allows to enter, withdraw, and record transactions.
4. The electronic ledger advises whether to buy or sell the coin, based on the record of transactions.
5. The electronic ledger has a login and registration interface.
6. The electronic ledger graphs your portfolio value and the history of your transactions.

# Criteria B: Design

## System Diagram

![CommSci](https://github.com/Rokyyz/unit-1CS/assets/134658259/a85865ac-47e9-48db-b8f7-35016ae7cfe5)


**Figure 1.** This is a system diagram, it starts with the input - the keyboard and it finishes with the output which is the terminal in Pycharm. The computer that is used to program this wallet is MacBook Air Retina, 13-inch 2018 (the specs are further listed in the diagram) with macOs Ventura Version 13.5.2. The code is coded in Pycharm 3.9.6.

## Flow Diagrams
**Fig. 2** This is the flow diagram for the login system

![IMG_1825](https://github.com/Rokyyz/unit-1CS/assets/134658259/815f53bf-79c1-4985-bb8d-6dd35ecdb1d5)

## Records of Tasks

| Task No | Planned Action        | Planned Outcome                                                                          | Time estimate | Target completion date | Criterion |
|---------|-----------------------|------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Create system diagram | To have a clear idea of the hardware and software requirements for the proposed solution | 10min         | Sep 24                 | B         |
| 2       | Create a login system | To have a flow diagram and the code for the login system                                 | 30min         | Sep 14                 | B, C      |

# Criteria C: Development

## Login System
My client requires a system to protect the private data. I thought about using a login system to accomplish this requirement using a if condition and the open command to work with a csv file.

As you can see in the flow diagram in **Fig 1**, in the first line I am defining a function called try_login, this function has two inputs of type string, and the output is a boolean representing True if the user logins correctly or false otherwise. Tjos os saved in the variable success. Then in line two... this is your work.

```.py

def try_login(name:str, password:str)-> bool:
    with open('users.csv', mode='r') as f:
        data = f.readlines()

    success = False
    for line in data:
        uname = line.split(',')[0]
        upass = line.split(',')[1].strip() # strip() removes \n
        if uname == name and upass == password:
            success = True
            break
    return success

```
