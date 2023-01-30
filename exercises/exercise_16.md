# Exercise 16

Use a list comprehension to square each odd number in a list. The list is input by a sequence of comma-separated numbers. >Suppose the following input is supplied to the program:

## Code
```python
lst = [str(int(i) ** 2) for i in input().split(",") if int(i) % 2]
print(",".join(lst))
```

## ChatGPT Explanation

This code takes an input, which is expected to be a comma-separated list of numbers, converts it into a list of strings, then it applies a list comprehension on it.

The list comprehension iterates over each element of the input list, checks if it is odd by checking if the integer representation of the element modulo 2 is non-zero. If it is odd, it takes the square of the element and converts it back to a string before appending it to the new list.

At the end, it uses the `join` method to join the elements of the new list with commas and prints it.