# python-practice
## repo of python practice for me to keep track of

## CodinGame
- https://www.codingame.com/ide/puzzle/mars-lander-episode-1
- https://www.codingame.com/ide/puzzle/temperatures
- https://www.codingame.com/training/medium/shadows-of-the-knight-episode-1

### My ASCII Art Puzzle Solution
___
```
import sys
import math

l = int(input())
h = int(input())
t = input()
row = [input() for i in range(h)]
for j in range(h):
    for i in t:
        asc = (ord(i.upper())-65) if i.isalpha() else 26
        print(row[j][(l*asc):(l*(asc+1))], end='')
    print()
```
    
___
