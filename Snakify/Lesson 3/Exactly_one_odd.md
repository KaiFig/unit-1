![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%203/Exactly_one_odd.jpg)

```.py
integer = int(input())
integer2 = int(input())
result = "NO"

if (integer % 2 == 1) or (integer2 % 2 == 1):
    result = "YES"
    
if (integer % 2 == 1) and (integer2 % 2 == 1):
    result = "NO"
    
print(result)
