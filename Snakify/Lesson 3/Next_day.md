![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%203/Next_day.jpg)

```.py
month = int(input())
day = int(input())
if month == 1 or month == 3 or month == 5 or month == 7 or month == 8 or month == 10 or month == 12:
    numdays = 31
if month == 2:
    numdays = 28
if month == 4 or month == 6 or month == 9 or month == 11:
    numdays = 30
    
if month<12 and numdays == day: 
    print(month+1)
    print(1) 
elif month == 12 and numdays == day:
    print(1)
    print(1)
else:
    print(month, day+1)
