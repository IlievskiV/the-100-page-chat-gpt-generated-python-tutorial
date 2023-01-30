# Exercise 21

A robot moves in a plane starting from the original point (0,0). The robot can move toward UP, DOWN, LEFT and RIGHT with a given steps. The trace of robot movement is shown as the following:

- UP 5
- DOWN 3
- LEFT 3
- RIGHT 2

The numbers after the direction are steps. Please write a program to compute the distance from current position after a sequence of movement and original point. If the distance is a float, then just print the nearest integer. Example: If the following tuples are given as input to the program:

## Code
```python
import math

x, y = 0, 0
while True:
    s = input().split()
    if not s:
        break
    if s[0] == "UP":  # s[0] indicates command
        x -= int(s[1])  # s[1] indicates unit of move
    if s[0] == "DOWN":
        x += int(s[1])
    if s[0] == "LEFT":
        y -= int(s[1])
    if s[0] == "RIGHT":
        y += int(s[1])
        # N**P means N^P
dist = round(
    math.sqrt(x ** 2 + y ** 2)
)  # euclidean distance = square root of (x^2+y^2) and rounding it to nearest integer
print(dist)
```

## ChatGPT Explanation

This code snippet is a Python program that calculates the distance from the origin `(0,0)` to a point on the x-y plane. 

The program takes input as a series of commands `(UP, DOWN, LEFT, RIGHT)` and an integer value indicating the number of units to move in that direction. The input is repeatedly taken in a `while` loop until a blank input is given. 

The program keeps track of the `x` and `y` coordinates as the input commands are executed and then calculates the distance from the origin to the final point using the Pythagorean theorem (the square root of `x^2 + y^2`). The calculated distance is rounded off and then printed.