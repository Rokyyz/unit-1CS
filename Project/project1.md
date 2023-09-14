# Crypto Wallet

![image](https://github.com/Rokyyz/unit-1CS/assets/134658259/4d5644ab-a44d-4118-91e1-7a47efac85c7)


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
I will design and make a ———— for a client who is ———. The ——– will about ———— and is constructed using the software ———. It will take  ———- to make and will be evaluated according to the criteria ———.

** add a description of your coin and citation (MLA)**

At its heart, Dogecoin is the accidental crypto movement that makes people smile! It is also an opensource peer-to-peer cryptocurrency that utilises blockchain technology, a highly secure decentralised system of storing information as a public ledger that is maintained by a network of computers called nodes. 

https://dogecoin.com/ 


Justify the tools/structure of your solution

## Success Criteria


1. The electronic ledger is a text-based software (Runs in the Terminal).
2. The electronic ledger display the basic description of the cyrptocurrency selected.
3. The electronic ledger allows to enter, withdraw and record transactions.
4. The electronic ledger advises whether to buy or sell the coin
5. The electronic ledger displays a login page with encrypted password
6. The electronic ledger graphs/makes a table of your portfolio value

# Criteria B: Design

## System Diagram

![IMG_1819](https://github.com/Rokyyz/unit-1CS/assets/134658259/cf396afe-d75c-4077-95a4-d39495cf2c74)

**Figure 1.** This is a system diagram, it starts with the input - the keyboard and it finishes with the output which is the terminal in Pycharm. The computer that is used to program this wallet is MacBook Air Retina, 13-inch 2018 (the specs are further listed in the diagram) with macOs Ventura Version 13.5.2. The code is coded in Pycharm 3.9.6.

## Flow Diagrams
**Fig. 2** This is the flow diagram for the login system

![IMG_1823](https://github.com/Rokyyz/unit-1CS/assets/134658259/748b54de-49f4-4e7c-9389-3560630d037c)

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
