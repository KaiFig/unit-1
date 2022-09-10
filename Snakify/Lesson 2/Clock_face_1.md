

```.py
h = int(input())
m = int(input())
s = int(input())

s += h*3600 + m *60

angle = s/43200
print(angle*360)
