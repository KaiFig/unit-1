![Tax calculator](https://github.com/KaiFig/unit-1/blob/main/Tax_calculator.jpg)

```.py
print("Welcome to the online tax calculator!")
salary = int(input("What is your salary? "))
if 0<=salary<=10000:
    tax = salary*0.05
if 10001<=salary<=50000:
    tax = salary*0.1
if 50001<=salary<=100000:
    tax = salary*0.15
if salary>100001:
    tax = salary*0.25
print("Your tax is " + str(tax) + " USD")
print("Thank you for using our website!")
