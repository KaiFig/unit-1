![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%203/Minimum_of_three_numbers.jpg)

```.py
integera = int(input())
integerb = int(input())
integerc = int(input())

if integera<integerb and integera<integerc:
    print(integera)
if integerb<integera and integerb<integerc:
    print(integerb)
if integerc<integera and integerc<integerb:
    print(integerc)
