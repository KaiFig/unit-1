```.py

h = int(input())
m = int(input())
s = int(input())
h2 = int(input())
m2 = int(input())
s2 = int(input())

hours = h2 - h
minutes = m2 - m
seconds = s2 - s

total = (hours*3600) + (minutes*60) + seconds
print(total)
