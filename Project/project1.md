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
**Fig. 2** 

![Com Sci](https://github.com/Rokyyz/unit-1CS/assets/134658259/a7735c18-e1d9-4323-a579-f41fc46fbd30)

**Fig. 3** 

![Com Sci 2](https://github.com/Rokyyz/unit-1CS/assets/134658259/3b0c992d-fb24-45fb-8da4-edae60eb649f)


**Fig. 4** 

![Com Sci 3](https://github.com/Rokyyz/unit-1CS/assets/134658259/61f4ea62-b912-4c10-b511-0a4d7bdfa3fe)


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
