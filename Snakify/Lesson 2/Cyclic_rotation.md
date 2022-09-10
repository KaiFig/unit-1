![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%202/Cyclic_rotation.jpg)

```.py
number1 = int(input())
thousand = number1//100
tens = number1%100
tens2 = tens*100
print(thousand+tens2)
