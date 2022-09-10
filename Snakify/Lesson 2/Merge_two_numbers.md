

```.py
number1 = int(input())
number2 = int(input())
tennumber1 = number1//10
onenumber1 = number1%10
tennumber2 = number2//10
onenumber2 = number2%10
thousand = tennumber1*1000
hundred = tennumber2*100
ten = onenumber1*10
print(thousand + hundred + ten + onenumber2)
