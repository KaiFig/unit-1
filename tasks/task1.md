![Solution](https://github.com/KaiFig/unit-1/blob/main/task1_test.jpg)


Question 1: 
Sierra 
Started in 1992 after the non-proliferation treaty
Ended arms race
US didn’t follow the non-proliferation treaty
Using sierra to try to model the reliability of the nuclear weapons arsenal for the US
Models changes due to age to see if anything will break (Job gets harder the older they get)
Part of the stockpile stewardship program

Question 2: 
The benefits of these supercomputers is that they enable us to figure out problems that are too complex for normal computers or us. Therefore, they can find life saving solutions to problems. However, one drawback is the risk of these machines falling into the wrong hands, that could create enormous problems for society. 

Question 3:
In Japan the most advanced computer is Fugaku. It is located in the Riken Center for Computational Science in Kobe. It has a speed of 442 PFLOPS and it has been used for COVID research and meteorological forecasting. 


```.py

#Part 1: 

lockernum = 2400
colors1 = ["blue", "red", "white", "yellow"]
blue = "\33[0;34m"
red = "\33[0;31m"
white = "\33[0;37m"
yellow = "\33[0;33m"
colors = [blue, red, white, yellow]
for locker in range(1,lockernum+1):
    color2 = (colors1[locker%4])
    color = (colors[locker%4])
    print(f"{color}Locker no.{locker} is {color2.center(50,'.')}")
    
#Part 2: 
locker = input("Enter your locker number: ")
number_lockers = 2400
max_num_tries = 5
i = locker

if int(locker)<2400 and int(locker)%4 == 0:
    colors = ["blue", "red", "white", "yellow"]
    color = colors[int(locker)%4]
    print(f"locker No {locker} is color {color.center(50, '.')}")
if int(locker)<2400 and int(locker)%4 == 1:
    colors = ["blue", "red", "white", "yellow"]
    color = colors[int(locker)%4]
    print(f"locker No {locker} is color {color.center(50, '.')}")
if int(locker)<2400 and int(locker)%4 == 2:
    colors = ["blue", "red", "white", "yellow"]
    color = colors[int(locker)%4]
    print(f"locker No {locker} is color {color.center(50, '.')}")
if int(locker)<2400 and int(locker)%4 == 3:
    colors = ["blue", "red", "white", "yellow"]
    color = colors[int(locker)%4]
    print(f"locker No {locker} is color {color.center(50, '.')}")

