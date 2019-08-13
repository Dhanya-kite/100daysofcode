## STATEMENT:   
### There was a set of cards with numbers from 1 to N. One of the card is now lost. Determine the number on that lost card given the numbers for the remaining cards.

### Given a number N, followed by N − 1 integers representing the numbers on the remaining cards (distinct integers in the range from 1 to N). Find and print the number on the lost card.
#### Sample I/O:
```
Example input
5
3
5
2
1

Example output
4
```
### Program:
```
limit = int(input(""))
List = [int(input()) for i in range(1 , limit)] 
for i in range (1 , limit + 1):
  if List.count(i) == 0:
    print(i)
```
