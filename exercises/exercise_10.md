# Exercise 10

Write a program that accepts a sequence of whitespace separated words as input and prints the words after removing all duplicate words and sorting them alphanumerically.

## Code

```python
word = sorted(
    list(set(input().split()))
)
print(" ".join(word))
```

## ChatGPT Explanation

This code is a simple program that takes a string of words as input, sorts them in alphabetical order and removes any duplicates, and then prints out the unique and sorted words as a string.

The first line of code uses the `input()` function to get user input, which is expected to be a string of words, and the `split()` method to convert the input string into a list of words by splitting it at each space.

Then it converts the list of words into a set with the `set()` method, which removes any duplicates. Then the set is converted back to a list with `list()` method.

The second line sorts the list of words using the `sorted()` method. This sorts the list in alphabetical order.

The final line of code uses the `join()` method to join the list of words into a string of words separated by space, and then prints it out.