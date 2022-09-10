![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%203/Chess_board_same_color.jpg)

```.py
positionx1 = int(input())
positiony1 = int(input())
positionx2 = int(input())
positiony2 = int(input())

if (positionx1+positiony1)%2==0 and (positiony2+positionx2)%2==0:
    print("YES")
elif (positionx1+positiony1)%2!=0 and (positionx2+positiony2)%2!=0:
    print("YES")
else:
    print("NO")
