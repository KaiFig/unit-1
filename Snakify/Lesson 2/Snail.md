![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%202/Snail.jpg)

```.py
import math

h = int(input()) #10
a = int(input()) #3
b = int(input()) #2

total = a-b #1
print(math.ceil((h-a)/(total)+1))
