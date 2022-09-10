![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%203/Distance_to_closest_point.jpg)

```.py
point1 = abs(int(input()))
point2 = abs(int(input()))
point3 = abs(int(input()))

if abs(point2-point1)<abs(point3-point1):
    print(abs(point2-point1))
else:
    print(abs(point3-point1))
