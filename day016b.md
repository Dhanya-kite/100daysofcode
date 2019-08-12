## STATEMENT:
### In mathematics, the factorial of an integer n, denoted by n! is the following product:   n! = 1 × 2 × … × n

For the given integer n calculate the value 

1! + 2! + 3! + ... + n!

Try to discover the solution that uses only one for-loop. And don't use math module in this exercise.
#### Sample I/O:
```
Example input
4

Example output
33
```
### Program:
```
n = int(input(""))
s = 0
factorial = 1

for i in range(1,n + 1):
       factorial = factorial * i
       s = s + factorial
print(s)
```
