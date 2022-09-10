![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%203/Chess_board_black_sq.jpg)

```.py
positionx = int(input())
positiony = int(input())

if (positionx+positiony)%2==0:
    print("BLACK")
else:
    print("WHITE")
