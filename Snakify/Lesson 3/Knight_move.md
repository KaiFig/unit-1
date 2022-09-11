![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%203/Kinght_move.jpg)

```.py
x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())

if (abs(x2-x1) ==2 or abs(y2-y1) == 2) and (abs(x2-x1) ==1 or abs(y2-y1) == 1):
    print("YES")
else:
    print('NO')
