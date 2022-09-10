

```.py
year = int(input()) #1965
convert_year = year//100
if year%100==0:
    print(convert_year)
else:
    print(convert_year+1)
