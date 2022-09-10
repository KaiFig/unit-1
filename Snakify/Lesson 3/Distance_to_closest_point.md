

```.py
point1 = abs(int(input()))
point2 = abs(int(input()))
point3 = abs(int(input()))

if abs(point2-point1)<abs(point3-point1):
    print(abs(point2-point1))
else:
    print(abs(point3-point1))
