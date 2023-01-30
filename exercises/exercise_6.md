# Exercise 6

Write a program that calculates and prints the value according to the given formula:

`Q = Square root of [(2 _ C _ D)/H]`

Following are the fixed values of C and H:

- C is 50. H is 30.

D is the variable whose values should be input to your program in a comma-separated sequence. For example Let us assume the following comma separated input sequence is given to the program:

## Code
```python
from math import sqrt

C, H = 50, 30

def calc(D):
    return sqrt((2 * C * D) / H)

print(",".join([str(int(calc(int(i)))) for i in input().split(",")]))
```

## ChatGPT Explanation

This code is a simple program that takes a string of comma-separated values as input, performs some calculations on each of the values, and then prints the result as a string of comma-separated values.

The first line of code imports the `sqrt()` function from the math module, which is used to calculate the square root of a number.

The next two lines define two constants, `C` and `H`, which are used in the calculations.

The following function `calc(D)` takes a parameter `D` and returns the result of the calculation `sqrt((2 * C * D) / H)`

The final line of code uses the `input()` function to get user input, which is expected to be a string of comma-separated values. It then uses the `split()` method to convert the input string into a list of strings by splitting it at each comma.

It then creates a list comprehension that iterates over the list of input values, calls the `calc()` function on each input value, which returns a float, and then converts the float to an int using the `int()` function. Then it uses the `join()` method to join the list of integers into a string of comma-separated values and prints it out.