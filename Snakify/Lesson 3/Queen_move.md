![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%203/Queen_move.jpg)

```.py
x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())

if abs(x2-x1)==abs(y2-y1):
    print("YES")
elif x1==x2 or y1==y2:
    print("YES")
else:
    print("NO")

