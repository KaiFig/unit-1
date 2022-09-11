

```.py
month = int(input())

if month == 1 or month == 3 or month == 5 or month == 7 or month == 8 or month == 10 or month == 12:
    print(31)
if month == 2:
    print(28)
if month == 4 or month == 6 or month == 9 or month == 11:
    print(30)
