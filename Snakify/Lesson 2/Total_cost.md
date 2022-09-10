![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%202/Total_cost.jpg)

```.py
# Read an integer:
a = int(input())
# Read a float:
b = float(input())
# Print a value:
N = int(input())
total_dollar = 0
total_cents = b*N
total_dollar += a*N
while total_cents>=100: #200
    total_cents -= 100
    total_dollar += 1 #9
print(total_dollar)
print(total_cents)
