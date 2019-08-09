### Digit in Number
Read two inputs. 
The first input is a digit. 
The second input is a number. 

Is the digit present in the number? If yes, return True.
If no, return False.
```
INPUT
1
100
OUTPUT
True

INPUT
4
234
OUTPUT
True

INPUT
1
2000
OUTPUT
False
```
### Program:

digit_d = input("")

num_n = input("") 

if (digit_d in num_n):

print("True")

else:

print("False")
  


for digit in num_n:

if digit == digit_d:

print("True")

break

else:

print("False")

break
    
    

print(digit_d in num_n)
