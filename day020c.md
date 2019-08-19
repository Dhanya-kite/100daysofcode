## STATEMENT:
### Given a list of non-zero integers, find and print the first adjacent pair of elements that have the same sign. If there is no such pair, print 0.
#### Sample I/O:
```
Example input #1
-1 2 3 -1 -2

Example output #1
2 3

Example input #2
1 -3 4 -2 1

Example output #2
0
```
### Program:
```
List = [int(s) for s in input().split()]
for i in range(1 , len(List)):
  if List[i] * List[i-1] > 0:
    print(str(List[i - 1]) + ' ' + str(List[i]))
    break
  elif i == len(List) - 1:
    print("0")
```
