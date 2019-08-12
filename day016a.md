## STATEMENT:
### For the given integer N calculate the following sum:   1³ + 2³ + ... + N³
#### Sample I/O:
```
Example input
3

Example output
36
```
### Program:
```
num = int(input(""))
Sum = 0

for i in range(1, num+1): 
  Sum += i * i * i 
print(Sum)
```
