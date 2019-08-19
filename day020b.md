## STAEMENT:
### Given a list of numbers, find and print all its elements that are greater than their left neighbor.
#### Sample I/O:
```
Example input
1 5 2 4 3

Example output
5 4

```
### Program:
```
List = [int(s) for s in input().split()]
for i in range(1, len(List)):
  if List[i - 1] < List[i]:
    print(List[i])
```
