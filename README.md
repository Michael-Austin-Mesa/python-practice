# python-practice
## repo of python practice for me to keep track of

## CodinGame
- https://www.codingame.com/ide/puzzle/mars-lander-episode-1
- https://www.codingame.com/ide/puzzle/temperatures
- https://www.codingame.com/training/medium/shadows-of-the-knight-episode-1

### My Mars Lander Episode 1 Solution
___
```
import sys
import math

# Auto-generated code below aims at helping you parse
# the standard input according to the problem statement.

surface_n = int(input())  # the number of points used to draw the surface of Mars.
for i in range(surface_n):
    # land_x: X coordinate of a surface point. (0 to 6999)
    # land_y: Y coordinate of a surface point. By linking all the points together in a sequential fashion, you form the surface of Mars.
    land_x, land_y = [int(j) for j in input().split()]

# game loop
while True:
    # h_speed: the horizontal speed (in m/s), can be negative.
    # v_speed: the vertical speed (in m/s), can be negative.
    # fuel: the quantity of remaining fuel in liters.
    # rotate: the rotation angle in degrees (-90 to 90).
    # power: the thrust power (0 to 4).
    x, y, h_speed, v_speed, fuel, rotate, power = [int(i) for i in input().split()]

    # Write an action using print
    # To debug: print("Debug messages...", file=sys.stderr, flush=True)
    if v_speed < -40:
        power = 4

    # 2 integers: rotate power. rotate is the desired rotation angle (should be 0 for level 1), power is the desired thrust power (0 to 4).
    print(f"{rotate} {power}")

```
___
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
