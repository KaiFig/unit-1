![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%203/Leap_year.jpg)

```.py
year = int(input())
if (year%4) == 0 and (year%100) != 0:
    print("LEAP")
elif (year%400) == 0:
    print("LEAP")
else:
    print("COMMON")
