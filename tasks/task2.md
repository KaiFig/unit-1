```.py

from My_library import validate_int_input, colors, end_code, bold
import math
welcome_msg = "Welcome to the EV Calculator".center(50, "=")
print(f"{colors[4]}{welcome_msg}{end_code}")
prompt_msg = "Please enter an option [1-4]"
print("Options".center(50))
menu = """1. Average time per kWh
2. Total kWh
3. Total charge time
4. Show all data
"""
print(menu)

x = input(prompt_msg)

option = validate_int_input(x)
while option>4 or option < 1:
    option = validate_int_input(f" {colors[1]}Error {prompt_msg}{end_code}")

#option 4:show all data
#With open(file_name, mode) Mode can be r:read (makes new file) w:write a:append (adds)
with open("charging_log.csv", "r") as file:
    ev_logs = file.readlines()

if option == 4:
    print(f"{bold[2]},4. showing all data {end_code}")  # Strip removes the\n
    index = 0
    for log in ev_logs:
        if index>0:
            print(f"No.{index}:{log}", end ="") #Strip removes the\n
        index += 1
if option == 2:
    index = 0
    total_energy = 0
    for log in ev_logs:
        if index > 0:
            values = log.split(",")
            date = values[0]
            energy = values[1]
            time = values[2]
            total_energy += float(energy[0:5])
        index += 1
    print(f"{colors[2]}The total energy charged is {total_energy}kWh")

if option == 3:
    index = 0
    total_hrs1 = 0
    total_energy1 = 0
    total_energy2 = 0
    total_hrs = 0
    total_minutes = 0
    total_seconds = 0
    for log in ev_logs:
        if index > 0:
            secs = log.split(":")
            time = secs[0]
            time1 = secs[2]
            time2 = secs[1]
            total_hrs1 += float(time[17:19])
            total_energy1 += float(time1[0:2])
            total_energy2 += float(time2[0:2])

        index += 1
    total_hrs += (total_hrs1 + total_energy2 // 60)
    total_minutes += (total_energy2%60 + total_energy1//60)
    if total_minutes > 59:
        total_hrs += total_minutes//60
        total_seconds += (total_energy1 % 60)
        total_minutes == (total_minutes%60)
        print(f"{colors[6]}{total_hrs} hours {total_minutes%60} minutes and {total_seconds} seconds")
    else:
        total_seconds += (total_energy1%60)
        total_minutes == total_minutes//60
        print(f"{colors[6]}{total_hrs} hours {total_minutes%60} minutes and {total_seconds} seconds")



if option == 1:
    index = 0
    total_energy = 0
    total_hrs1 = 0
    total_energy1 = 0
    total_energy2 = 0
    total_hrs = 0
    total_minutes = 0
    total_seconds = 0
    for log in ev_logs:
        if index > 0:
            values = log.split(",")
            date = values[0]
            energy = values[1]
            time = values[2]
            total_energy += float(energy[0:5])
        elif index > 0:
            secs = log.split(":")
            time = secs[0]
            time1 = secs[2]
            time2 = secs[1]
            total_hrs1 += float(time[17:19])
            total_energy1 += float(time1[0:2])
            total_energy2 += float(time2[0:2])

        index += 1
    total_hrs += (total_hrs1 + total_energy2 // 60)
    total_minutes += (total_energy2 % 60 + total_energy1 // 60)
    if total_minutes < 30:
        total_hrs += total_minutes // 60
        total_seconds += (total_energy1 % 60)
        total_minutes == (total_minutes % 60)
        total = ((total_hrs/3600)+(total_minutes/60)+total_seconds)
        persec = total_energy/126000
        times = 1/persec
        hours = ((1*times)//3600)
        mins = (((1*times)%3600)//60)
        secs1 = (((1*times)%3600)%60)
        print(f"{colors[3]}{hours} hour {mins} minutes and {math.ceil(secs1)} seconds to charge 1 kWh")
    else:
        total_seconds += (total_energy1 % 60)
        total_minutes == total_minutes % 60
        total = ((total_hrs/3600)+(total_minutes/60)+total_seconds)
        persec = total_energy/126000
        times = 1/persec
        hours = ((1 * times) // 3600)
        mins = (((1 * times) % 3600) // 60)
        secs1 = (((1*times)%3600)%60)
        print(f"{colors[4]}{hours} hour {mins} minutes and {math.ceil(secs1)} seconds to charge 1 kWh")
