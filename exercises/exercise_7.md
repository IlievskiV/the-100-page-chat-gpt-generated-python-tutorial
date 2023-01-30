# Exercise 7

Write a program which takes 2 digits, X, Y as input and generates a 2-dimensional array. The element value in the i-th row and j-th column of the array should be i_j.

## Code
```python
x, y = map(int, input().split(","))
lst = [[i * j for j in range(y)] for i in range(x)]
print(lst)
```

## ChatGPT Explanation

This code is a simple program that takes two integers as input, separated by a comma and creates a list of lists (also known as a 2D list) by using a nested list comprehension.

The first line of code uses the `input()` function to get user input, which is expected to be two integers separated by a comma.
It then uses the `split()` method to separate the input string at the comma and the `map()` function to convert the resulting two strings into integers and assigns them to the variables `x`, `y`.

The second line of code creates a list of lists called `lst` using a nested list comprehension. The outer list comprehension iterates over the range of `x`, and the inner list comprehension iterates over the range of `y`, and it creates a new list of integers where each integer is the product of the outer loop variable and the inner loop variable.

The last line of code prints out the list of lists.