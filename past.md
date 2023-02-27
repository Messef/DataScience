
WRITE A PROGRAM THAT DISPLAYS THE LARGEST NUMBER IN A LIST {
import random

list= [53, -42, -90, 124, 10, 8] #n, total nums, is 6
def findGreatest(list, n):
    counter = 1
    greatest = list[0]
    while counter < n: 
        num=list[counter]
        if num > greatest:
            greatest = num
        else:
            pass
        counter+=1

    else: print(greatest)

        
findGreatest(list, 6)
}




WRITE A PROGRAM THAT DISPLAYS THE SMALLEST NUMBER IN A LIST {
list= [53, -42, -90, 124, 10, 8] #n, total nums, is 6
def findLowest(list, n):
    counter = 1
    lowest = list[0]
    while counter < n: 
        num=list[counter]
        if num < lowest:
            lowest = num
        else:
            pass
        counter+=1

    else: print(lowest)

        
findLowest(list, 6)


}



Manually sort a list {
list= [24, 3, 16, 154, 23] #n, total nums, is 6
lowest = 0
def findLowest(list, n):
    global lowest
    counter = 1
    lowest = list[0]
    while counter < n: 
        num=list[counter]
        if num < lowest:
            lowest = num
        else:
            pass
        counter+=1

findLowest(list, len(list))

def sortList(list):
    global lowest
    newList = []
    while len(list)!=0:
        findLowest(list, len(list))
        list.remove(lowest)
        newList.append(lowest)
    else: print(newList)
sortList(list)

}




'''Manually sort a list'''
'''
list= [24, 3, 16, 154, 23] #n, total nums, is 6
lowest = 0
def findLowest(list, n):
    global lowest
    counter = 1
    lowest = list[0]
    while counter < n: 
        num=list[counter]
        if num < lowest:
            lowest = num
        else:
            pass
        counter+=1

findLowest(list, len(list))

def sortList(list):
    global lowest
    newList = []
    while len(list)!=0:
        findLowest(list, len(list))
        list.remove(lowest)
        newList.append(lowest)
    else: print(newList)
sortList(list)
'''
time = input("\nFirst time: ")
time2 = input("\nSecond time(0 if nothing): ")
op = input("\nOperation: ")

percent=input("\nWhat percent? ")

perc, perc1=0, 0

def convert(time, time2):

    global perc,perc1

    if len(time)==4: 
        perc = int(time[0:2])*60

        perc+=int(time[2])+int(time[3])

        print(f"{int((int(perc)*int(percent))/100)} minutes")

    else: 
        perc = int(time[0])*60

        print(perc)

        perc+=int(time[1])+int(time[2])

        print(f"{int((int(perc)*int(percent))/100)} minutes")

    if len(time2)!=1: 
        if len(time2)==4: 
            perc1 = int(time[0:2])*60

            perc1+=int(time[2])+int(time[3])

            print(f"{int( ( int(perc1) * int(percent) )/100)} minutes")
        else: 
            perc1 = int(time2[0])*60

            perc+=int(time2[1])+int(time2[2])

            print(f"{int((int(perc1)*int(percent))/100)} minutes")



def TimeCalc(time, time2, op):
    global perc, perc1, percent
    convert(time, time2)
    if op=="-": return perc-perc1
    elif op=="+": return perc+perc1
if op=="-" or op=="+": TimeCalc(time, time2, op)
else: convert(time, time2)
'''
    elif time2!=0: 

        if op == "-":

            convert(time, time2)

            final=perc-perc1

        elif op == "+":

            convert(time, time2)

            final=perc+perc1

TimeCalc(time, time2, op)'''

'''


'''
#https://docs.google.com/document/d/1Z8HdKJcSbUAu3WtawLHWQa6iWMmn2JMktL5TLD4E-zY/edit
import statistics

list = [1, 2, 3, 4, 5]
print(f"Standard Deviation is {statistics.median(list)} of the list {list}") '''
'''
Grade checker
a = int(input("Enter ur grade: "))
if a>95:
    print("that's a really good grade!")
elif a<85 and a>75: 
    print("disappointment")
elif a<95 and a>85: 
    print("j do better next time, okay? ")
elif a<75 and a>65: 
    print("How the hell? ")
else: print("you're dumb as heck ")
'''
'''
number=int(input("put a number: "))
divisor=int(input('put a divisor '))
interval=divisor
nums=[]
nums.append(divisor)

while divisor<number:
    divisor+=interval
    if divisor<=number: 
        nums.append(divisor)
    else: pass

else: 
    if len(nums)>1: print(f'there are {len(nums)} intervals of {interval} in {number}')
    else: print(f'there are {len(nums)} intervals of {interval} in {number}')
'''
'''
Importing files: 
test.py
import main 
binary = input("do u wanna get degrees or radians: ")
if binary=="radians":
    converttoR = float(input("give degrees to get to radians: "))
    while converttoR>0: 
        print(main.Radians(converttoR))
        converttoR = float(input("give degrees to get to radians: "))

    else: quit()
else: 
    converttoD = float(input("give radians to get to degrees: "))
    while converttoD>0: 
       print(main.Degrees(converttoD))
       converttoD = float(input("give degrees to get to radians: "))
    else: quit()
main.py
'''
Remember to:
1.) Put Inputs as integers
2.) Make sure your program has an output(as either return or print)
3.) 

'''
import math
def Radians(degrees):
    answer = degrees/180
    answer*=math.pi
    return answer
def Degrees(radians):
    radians *=180
    radians/=math.pi
    return radians
'''

