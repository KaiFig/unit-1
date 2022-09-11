![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%203/Chocolate_bar.jpg)

```.py
n = int(input())
m = int(input())
k = int(input())

if (k%n == 0 and k/n < m) or (k%m == 0 and k/m < n):
    print("YES")
else:
    print("NO")
