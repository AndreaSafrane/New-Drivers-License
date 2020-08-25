# New-Drivers-License
You have to get a new driver's license and you show up at the office at the same time as 4 other people. The office says that they will see everyone in alphabetical order and it takes 20 minutes for them to process each new license. All of the agents are available now, and they can each see one customer at a time. How long will it take for you to walk out of the office with your new license?

#Input Format 
#string of your name, an integer of the number of available agents, and a string of the other four names separated by spaces.

#Output Format 
#integer of the number of minutes that it will take to get your license.

my_name = input()
agents = int(input())
people = input()

list = people.split()
list.append(my_name)
list.sort()

from math import *

for i in range(len(list)):
    if list[i] == my_name:
        time = floor(i / (agents))
        time = (before * 20) + 20
        
print(int(time))
