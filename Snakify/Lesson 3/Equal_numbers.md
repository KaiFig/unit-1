

```.py
integer1 = int(input())
integer2 = int(input())
integer3 = int(input())

if integer1==integer2==integer3:
    print(3)
elif integer1==integer2 or integer1==integer3 or integer2==integer3:
    print(2)
else:
    print(0)
