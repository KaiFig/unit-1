![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%202/Reverse_three_digits.jpg)

```.py
a = int(input())
b = a//100
c = a%10
d = a%100
e = d//10

hundred = c*100
ten = e*10

print(hundred+ten+b)
