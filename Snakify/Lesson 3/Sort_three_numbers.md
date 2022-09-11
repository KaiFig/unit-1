![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%203/Sort_three_numbers.jpg)

```.py
num1 = int(input())
num2 = int(input())
num3 = int(input())

if num1<=num2<=num3:
    print(num1)
    print(num2)
    print(num3)
elif num2<=num3<=num1:
    print(num2)
    print(num3)
    print(num1)
elif num3<=num2<=num1:
    print(num3)
    print(num2)
    print(num1)
elif num1<=num3<=num2: 
    print(num1)
    print(num3)
    print(num2)
elif num3<=num1<num2:
    print(num3)
    print(num1)
    print(num2)
elif num2<=num1<=num3:
    print(num2)
    print(num1)
    print(num3)
