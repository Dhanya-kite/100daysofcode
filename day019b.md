## STATEMENT:
### Given a string in which the letter h occurs at least twice, reverse the sequence of characters enclosed between the first and last occurrences of it.
#### Sample I/O:
```
Example input
In the hole in the ground there lived a hobbit

Example output
In th a devil ereht dnuorg eht ni eloh ehobbit

```
### Program:
```
s = input()

s1 = (s[s.find('h'):s.rfind('h')])
print(s[:s.find('h')+1] + s1[::-1]+ s[s.rfind('h')+1:])
```
