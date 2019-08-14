## STATEMENT:
### The Missing Spy Plane
The Indian Air Force (IAF)  is using more than 10,000 spy planes to  
go across LoC to scout for terrorist camps in Pakistan. Whenever a spy   
plane takes off for reconnaissance, the Plane ID is added to a list.  
Whenever the plane returns, the ID is again added to the same list.   

One spy plane alone has gone missing, so its ID was not added to the  
list a second time.  By the way, IDs are not guaranteed to be  
sorted or sequential.   

1. Given a list of plane IDs, write a program to print out the ID of 
the missing spy plane. 
2. If no plane is found missing, then print "All arrived!"  

#### Bonus 
2. The IAF is very keen to have the most efficient algorithm / solution.   
It wants one program that can finish within 10 milliseconds, even when   
there are more than 10 lakh sorties across the LoC by the spy planes,  
i.e. each spy plane might make upto 100+  visits across the LoC. 
#### Sample I/O:
```
INPUT
6
10001
10002
10003
10001
10003
10002

OUTPUT
All arrived!

INPUT
5
11100
11200
11300
11200
11300

OUTPUT
11100

```
### Program:
```
num = int(input(""))
List = [int(input()) for i in range(num)]
flag = 0
for i in range(num):
  if (List[i] != 0):
    count = 0
    for j in range(i + 1 , num):
      if (List[i] == List[j]):
        List[j] = 0
        count = 1
        break
    if (count == 0):
      flag = 1
      print(List[i])
if (flag == 0):
  print("All arrived!")
```
