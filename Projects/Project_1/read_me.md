# Crypto Wallet

![Gif](https://github.com/KaiFig/unit-1/blob/main/Projects/Project_1/avalanche-avax.gif)
# Criteria A: Planning

## Problem definition

Ms. Sato is a local trader who is interested in the emerging market of cryptocurrencies. She has started to buy and sell electronic currencies, however at the moment she is tracking all her transaction using a ledger in a spreadsheet which is starting to become burdensome and too disorganized. It is also difficult for Ms Sato to find past transactions or important statistics about the currency. Ms Sato is in need of a digital ledger that helps her track the amount of the cryptocurrency, the transactions, along with useful statistics. 

Apart for this requirements, Ms Sato is open to explore a cryptocurrency selected by the developer.

## Proposed Solution

Design statement:
I will design and make a digital ledger for a client who is a local trader. The ledger  will inform and organize her crypto investments and is constructed using the software python. It will take 30 hours to make and will be evaluated according to the criteria ———.

** add a description of your coin and citation **
Kai: Avalanche 

## Rationale for solution

  In this project I will be coding in python to create the crypto wallet for Ms. Sato. This is because python is quite a simple coding language compared to other languages and with that I wil be able to progress quicker on this project. Additionally, in this computer science class, we have only learnt how to code in python so far. Therefore, if we weren't using python in this project it would be very hard and almost impossible to do a project at this level since it would require us to learn a completely new coding language. 
  
  In this project, I will be using PyCharm to help me code this crypto wallet. This is because we have been using PyCharm during this year to develop our coding skills. PyCharm points out the errors that we have and it also enables us to create different types of files which is of utmost importance in this project. Also, it organizes new python files and also makes it more efficient for us. This project requires us to use different types of files like .csv files so it is beneficial to base it all on a platform that enables us to do so. 
  
  Lastly, for this project, I have decided to make a digital wallet that runs in the Terminal because that is what the customer has requested. I have also decided to make it more secure by requiring a password to access and it makes sure that Ms. Sato can keep her cryptocurrency transactions organized. This way, Ms. Sato will be able to access all the information about her crypto transactions and still be assured that it will be safe 

## Success Criteria
1. The electronic ledger is a text-based software (Runs in the Terminal).
2. The electronic ledger display the basic description of the cyrptocurrency selected.
3. The electronic ledger allows to enter, withdraw and record transactions.
4. The electronic ledger will provide and display her transactions with a graph
5. The electronic ledger will be secure and require a password
6. The electronic ledger will display statistics (Deposit and Withdraw) of her account per month


# Criteria B: Design

## System Diagram

## Flow Diagrams


## Record of Tasks
| Task No | Planned Action                                                | Planned Outcome                                                                                                 | Time estimate | Target completion date | Criterion |
|---------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Create the design statement                                   | To have a clear idea of what is needed in this project                                                          | 10min         | Sep 24                 | A         |
| 2       | Create system diagram                                         | To have a clear idea of the hardware and software requirements for the proposed solution                        | 10min         | Sep 24                 | B         |
| 3       | Create a password file                                        | To make sure that the clients wallet is protected                                                                | 10min         | Oct 3                  | C         |
| 4       | Create three flow charts                                    | To have a clear understanding of what I need to do to code the entire project                                      | 30min         | Oct 1                  | B         |
| 5       | Create the success criteria                                 | To know what I should be aiming for with my code and how I should evaluate it                                      | 15min         | Sep 30                 | A         |
| 6       | Write the rationale for solution                            | Know exactly why I am choosing to do certain things                                                                | 20min         | Oct 1                  | A         |
| 7       | Create and test the password system                         | Make sure that the password protection is accurate and that it works for the user                                  | 30min         | Oct 2                  | C         |
| 8       | Create validation systems for every user input              | To make sure that the code won't crash and that the user experience is improved                                    | 1h 30 min     | Oct 3                  | C         |

## Test plan
| Tests | Input                                                         | Expected output
|-------|----------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------
|Password test| Correct password, incorrect password                     | f"{colors[1]}Please try again,{end_code} you have {max_num_tries} chances left ") or "Welcome to the digital ledger, Ms. Sato".center(70, "-")
|User selecting the option | Option between 1 and 3, option not between 1 and 3| Moves to option or (f"{colors[1]}Error please enter a valid input{end_code}")
|Start and message menu | None | print(f"{colors[4]}Welcome to the Avalanche crypto wallet!{end_code}")
| 
