## STATEMENT:
### Given a month - an integer from 1 to 12, print the number of days in it in the year 2017.
#### Sample I/O:
```
Example input #1
1
(January)

Example output #1
31

Example input #2
2
(February)

Example output #2
28
```
#### PRogram:
```
n = int(input(""))
if n == 4 or n == 6 or n == 9 or n == 11:
  print(30)
elif n == 2:
  print(28)
else:
  print(31)
```
