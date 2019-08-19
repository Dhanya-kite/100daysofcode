## STATEMENT:
### Given a list of distinct numbers, swap the minimum and the maximum and print the resulting list.
#### Sample I/O:
```
Example input
3 4 5 2 1

Example output
3 4 1 2 5

```
### Program:
```
a = [int(s) for s in input().split()]
max, min = a.index(max(a)), a.index(min(a))
a[max], a[min] = a[min], a[max]

print(a)
```
