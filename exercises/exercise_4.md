# Exercise 4

Write a program which accepts a sequence of comma-separated numbers from console and generate a list and a tuple which contains every number.Suppose the following input is supplied to the program:

## Code
```python
lst = input().split(",")
tpl = tuple(lst)

print(lst)
print(tpl)
```

## ChatGPT Explanation

This code snippet is a simple program that takes a string of comma-separated values as input, converts it to a list and then converts it to a tuple.

The first line of code is getting an input from the user and assigns it to the variable `lst`, The `split()` method is used to convert the input string into a list of strings by splitting it at each comma.

The next line of code creates a variable called `tpl`, and it uses the `tuple()` function to convert the `lst` variable from a list to a tuple.

The last two lines of code are using the `print()` function to display the `lst` variable and the `tpl` variable on the screen.