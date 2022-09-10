![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%202/Sum_of_digits.jpg)

```.py
a = int(input())
b = a%10
c = a%100
d = a%1000
e = c//10
f = d//100
number = (b+e+f)
print(number)
