

```.py
a = int(input())
b = int(input())

if a != 0 and b != 0:
    c = (b/a)
    if -1<c<1:
        print("no solution")
    else:
        print(c)
else:
    if a == 0 and b == 0:
        print("many solutions")
    else:
        print("no solution")

