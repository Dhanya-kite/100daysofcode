## STATEMENT:
### Given a list of numbers, find and print the elements that appear in it only once. Such elements should be printed in the order in which they occur in the original list.
#### Sample I/O:
```
Example input
4 3 5 2 5 1 3 5

Example output
4 2 1
```
### Program:
```
a = [int(s) for s in input().split()]

for i in a:
  if a.count(i) == 1:
    print(i, end=' ')
```
