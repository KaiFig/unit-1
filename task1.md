![Solution](https://github.com/KaiFig/unit-1/blob/main/task1_test.jpg)

```.py
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

