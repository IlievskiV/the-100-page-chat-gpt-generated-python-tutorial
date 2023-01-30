# Exercise 8

Write a program that accepts a comma separated sequence of words as input and prints the words in a comma-separated sequence after sorting them alphabetically.

## Code
```python
lst = input().split(",")
lst.sort()
print(",".join(lst))
```

## ChatGPT Explanation

This code is a simple program that takes a string of comma-separated values as input, sorts the values in alphabetical or numerical order, and then prints the sorted values as a string of comma-separated values.

The first line of code uses the `input()` function to get user input, which is expected to be a string of comma-separated values, and the `split()` method to convert the input string into a list of strings by splitting it at each comma.

The second line of code sorts the list of strings using the `sort()` method. This sorts the list in alphabetical order for strings and numerical order for numbers.

The final line of code uses the `join()` method to join the list of strings into a string of comma-separated values, and then prints it out.