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

Screen recording: https://drive.google.com/drive/folders/11DtlwHXdLAtS0auKOizCaDn1EOAdDpEN

```.py
from My_library import colors, end_code, validate_int_input


def validate_month(month):
    x = validate_int_input(month)
    month1 = x
    while not 0< month1 <13:
        month1 = input(f"Error please enter a valid month as a number")
        month1 = validate_int_input(month1)
    return int(month1)


def validate_numop(num_op):
    x = validate_int_input(num_op)
    num_op1 = x
    while not 0< num_op1 <4:
        num_op1 = input(f"{colors[1]}Error please enter a valid input{end_code}")
        num_op1 = validate_int_input(num_op1)
    return int(num_op1)


def validate_day(day):
    day1 = validate_int_input(day)
    day2 = day1
    while not 0 < (day2)<31:
        day2 = input(f"{colors[1]}Error please enter a valid day{end_code}")
        day2 = validate_int_input(day2)
    return int(day2)


def validate_day31(day):
    day2 = validate_int_input(day)
    day3 = day2
    while not 0<day3<32:
        day3 = input(f"{colors[1]}Error please enter a valid day{end_code}")
        day3 = validate_int_input(day3)
    return int(day3)


def validate_day28(day):
    day3 = validate_int_input(day)
    day4 = day3
    while not 0<day4<29:
        day4 = input(f"{colors[1]}Error please enter a valid day{end_code}")
        day4 = validate_int_input(day4)
    return int(day4)


def validateyear(year):
    year1 = validate_int_input(year)
    while not 2020<year1<2023:
        year1 = input(f"{colors[1]}Error please enter a valid year{end_code}")
        year1 = validate_int_input(year1)
    return int(year1)


def validate_withdrawl_deposit(item):
    item1 = validate_int_input(item)
    item2 = item1
    while not 0<item2<3:
        item2 = input(f"{colors[1]}Error please enter a valid number{end_code}")
        item2 = validate_int_input(item2)
    return int(item2)


def validate_repeat(repeat):
    x = validate_int_input(repeat)
    repeat1 = x
    while not 0<repeat1<3:
        repeat1 = input(f"{colors[1]}Error please enter a valid input{end_code}")
        repeat1 = validate_int_input(repeat1)
    return(repeat1)


def option_1():
    print("Deposit or Withdraw")
    with open("Digital_wallet.csv", "r") as file:
        wallet_data = file.readlines()
        last_data = wallet_data[len(wallet_data)-1]
        last_data1 = last_data.strip("\n")
        last_data_list = last_data1.split(',')
        recent_balance = int(last_data_list[5])
        select_item = "For Deposits, type 1, For withdraws, type 2: "
        item = input(select_item)
        validwith = validate_withdrawl_deposit(item)
        validnum = validwith
        with open("Digital_wallet.csv","a") as file:
            if int(validnum) == 1:
                print("Deposit money")
                month = input("Please enter the month of this transaction as a number ")
                x = validate_month(month)
                y = x
                if y == 1 or y == 3 or y == 5 or y == 7 or y ==8 or y == 10 or y == 12:
                    day = input("Please enter the day of this transaction as a number ")
                    validday = validate_day31(day)
                    finalday = validday
                elif y == 2:
                    day = input("Please enter the date of this transaction as a number ")
                    validday = validate_day28(day)
                    finalday = validday
                elif y == 4 or y == 6 or y == 9 or y == 11:
                    day = input("Please enter the date of this transaction as a number ")
                    validday = validate_day(day)
                    finalday = validday
                year = input("What is the year, 2021 or 2022?")
                validyear = validateyear(year)
                finalyear = validyear
                deposit = input("Deposit amount?")
                validdeposit = validate_int_input(deposit)
                validdeposit1 = validdeposit
                balance = (int(recent_balance)+int(validdeposit1))
                withdraw = 0
                total = (f"\n{y},{finalday},{finalyear},{validdeposit1},{withdraw},{balance}")
                file.write(total)
                print(f"{colors[6]}Thank you for using the crypto wallet, your money has been deposited{end_code}")
                print(f"{colors[5]}Your current balance is now {balance} AVX {end_code}")

            elif int(validnum) == 2:
                print("Withdraw money")
                month = input("Please enter the month as a number ")
                x = validate_month(month)
                y = x
                if y == 1 or y == 3 or y == 5 or y == 7 or y == 8 or y == 10 or y == 12:
                    day = input("Please enter the date of this transaction as a number ")
                    validday = validate_day31(day)
                    finalday = validday
                elif y == 2:
                    day = input("Please enter the date of this transaction as a number ")
                    validday = validate_day28(day)
                    finalday = validday
                elif y == 4 or y == 6 or y == 9 or y == 11:
                    day = input("Please enter the date of this transaction as a number ")
                    validday = validate_day(day)
                    finalday = validday
                year = input("What is the year, 2021 or 2022? ")
                validyear = validateyear(year)
                finalyear = validyear
                withdraw = input(f"Your current balance is {recent_balance} AVX. What is the withdraw amount? ")
                withdrawfinal = validate_int_input(withdraw)
                while not (int(withdrawfinal))<(int(recent_balance)):
                    withdrawfinal = input(f"{colors[1]}That number exceeds your current balance, please enter another number {end_code}")
                    withdrawfinal = validate_int_input(withdrawfinal)
                balance = (int(recent_balance)-int(withdrawfinal))
                deposit = 0
                total = (f"\n{y},{finalday},{finalyear},{deposit},{withdrawfinal},{balance}")
                file.write(total)
                print(f"{colors[6]}Thank you for using the crypto wallet, your money has been withdrawn.{end_code}")
                print(f"{colors[5]}Your current balance is now {balance} AVX {end_code}")


def option_2():
    year = input('Please enter a year, 2021 or 2022')
    year1 = validateyear(year)
    year2 = year1
    month_enter = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
    month_withdraw = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
    month = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October',
             'November', 'December']

    with open('Digital_wallet.csv', 'r') as f:
        date = f.readlines()
    for i in date:
        x = i.split(',')
        if x[2] == str(year2):
            month_enter[int(x[0]) - 1] = int(month_enter[int(x[0]) - 1]) + int(x[3])
            month_withdraw[int(x[0]) - 1] = int(month_withdraw[int(x[0]) - 1]) + int(x[4])

    for i in range(12):
        print(f'{month[i]},Deposits: {month_enter[i]}')
        print(f'{month[i]},Withdraw: {month_withdraw[i]}\n')


def option_3():
    print("Display transactions")
    year = input('Please enter year, 2021 or 2022')
    year1 = validateyear(year)
    month_transaction = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
    month = ['Jan |', 'Feb |', 'Mar |', 'Apr |', 'May |', 'Jun |', 'Jul |', 'Aug |', 'Sep |', 'Oct |', 'Nov |', 'Dec |']

    with open('Digital_wallet.csv', 'r') as f:
        date = f.readlines()
    for i in date:
        x = i.split(',')
        if x[2] == str(year1):
            month_transaction[int(x[0]) - 1] += 1
    for i in range(12):
        print(f'{month[i]} {("█ ") * month_transaction[i]}')


def password():
    with open("project1_password.csv", "r") as file:
        line = file.readlines()
        password = line[0]
        passwordin = input("Please enter your password: ")
        max_num_tries = 5
        while not password == passwordin and max_num_tries > 0:
            max_num_tries -= 1
            passwordin = input(f"{colors[1]}Please try again,{end_code} you have {max_num_tries} chances left ")
            if max_num_tries < 0:
                exit("The passwords were incorrect")
        welcome_msg = "Welcome to the digital ledger, Ms. Sato".center(70, "-")
        print(f"{colors[4]}{welcome_msg}{end_code}")

print(f"{colors[4]}Welcome to the Avalanche crypto wallet!{end_code}")
print(f"""{colors[2]}
░█████╗░██╗░░░██╗░█████╗░██╗░░░░░░█████╗░███╗░░██╗░█████╗░██╗░░██╗███████╗
██╔══██╗██║░░░██║██╔══██╗██║░░░░░██╔══██╗████╗░██║██╔══██╗██║░░██║██╔════╝
███████║╚██╗░██╔╝███████║██║░░░░░███████║██╔██╗██║██║░░╚═╝███████║█████╗░░
██╔══██║░╚████╔╝░██╔══██║██║░░░░░██╔══██║██║╚████║██║░░██╗██╔══██║██╔══╝░░
██║░░██║░░╚██╔╝░░██║░░██║███████╗██║░░██║██║░╚███║╚█████╔╝██║░░██║███████╗
╚═╝░░╚═╝░░░╚═╝░░░╚═╝░░╚═╝╚══════╝╚═╝░░╚═╝╚═╝░░╚══╝░╚════╝░╚═╝░░╚═╝╚══════╝{end_code}""")
password()
print(
    "Avalanche is a cryptocurrency and blockchain that was launched in 2021." " It is the native token of the avalanche blockchain."
    " It competes with ethereum with its scalability and transaction speed." " It can process up to 4500 transactions per second compared to Ethereum's 15.")
prompt_msg = "Please enter an option [1-3]"
x = 0
while x == 0:

    print("Options".center(50))
    menu = """
    1. Deposit or withdraw 
    2. Display statistics 
    3. Display transactions
    """
    print(menu)



    num_op = input(prompt_msg)
    validnumop = validate_numop(num_op)
    repeat = 0

    if int(validnumop) == 1:
        option_1()


        repeat = (input("Would you like to make another transaction? Enter 1 for yes, Enter 2 for no."))
        valid_repeat = validate_repeat(repeat)
        final_repeat = valid_repeat
        if final_repeat == 1:
            x = 0
        if final_repeat == 2:
            x += 1
            print(f"{colors[4]}Thank you for using the crypto wallet, have a nice day")
            exit()
    if int(validnumop) == 2:
        print("Display withdraws and deposits per month ")
        option_2()


        repeat = (input("Would you like to make another transaction? Enter 1 for yes, Enter 2 for no."))
        valid_repeat = validate_repeat(repeat)
        final_repeat = valid_repeat
        if final_repeat == 1:
            x = 0
        if final_repeat == 2:
            x += 1
            print(f"{colors[4]}Thank you for using the crypto wallet, have a nice day")
            exit()
    if int(validnumop) == 3:
        print("Display number of transactions per month ")
        y = "█"
        option_3()


        repeat = (input("Would you like to make another transaction? Enter 1 for yes, Enter 2 for no."))
        valid_repeat = validate_repeat(repeat)
        final_repeat = valid_repeat
        if final_repeat == 1:
            x = 0
        if final_repeat == 2:
            x += 1
            print(f"{colors[4]}Thank you for using the crypto wallet, have a nice day")
            exit()
