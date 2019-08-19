## STATEMENT:
### Given a list of numbers, print all its even elements. Use a for-loop that iterates over the list itself and not over its indices. That is, don't use range()
#### Sample I/O:
```
Example input
1 2 2 3 3 3 4

Example output
2 2 4
```
### Program:
```
List = [int(s) for s in input().split()]
for element in List:
    if element % 2 == 0:
        print(element)
```
