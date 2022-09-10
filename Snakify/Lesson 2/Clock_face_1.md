![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%202/Clock_face_1.jpg)

```.py
h = int(input())
m = int(input())
s = int(input())

s += h*3600 + m *60

angle = s/43200
print(angle*360)
