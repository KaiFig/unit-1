

```.py
a = int(input())
b = a//100
c = a%10
d = a%100
e = d//10

hundred = c*100
ten = e*10

print(hundred+ten+b)
