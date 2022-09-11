![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%203/White_pawn_move.jpg)

```.py
x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())

if y1 == 1:
    print("NO")
elif abs(x2-x1)>1:
    print("NO")
elif y2-y1 == 2 and y1 == 2 and x2-x1 == 0:
    print("YES")
elif y2-y1 == 1:
    print("YES")
elif (y2-y1) == 1 and abs(x2-x1) == 1:
    print("YES")
else:
    print("NO")
