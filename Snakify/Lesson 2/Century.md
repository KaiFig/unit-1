![Solution](https://github.com/KaiFig/unit-1/blob/main/Snakify/Lesson%202/Century.jpg)

```.py
year = int(input()) #1965
convert_year = year//100
if year%100==0:
    print(convert_year)
else:
    print(convert_year+1)
