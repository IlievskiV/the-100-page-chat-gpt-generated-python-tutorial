# Exercise 73
Please write a program to randomly generate a list with 5 even numbers between 100 and 200 inclusive.

## Code
```python
import random

resp = random.sample(range(100, 201, 2), 5)
print(resp)
```

## ChatGPT Explanation
This code snippet generates 5 random numbers from a range of even numbers between 100 and 201 (inclusive).

It starts by importing the `random` module, which contains a number of useful functions for generating random numbers, shuffling lists, and choosing random items from a list.

Next, the line `resp = random.sample(range(100, 201, 2), 5)` generates a list of 5 random numbers from a range of even numbers between 100 and 201 (inclusive).

The `range(100, 201, 2)` function generates a list of all even numbers between 100 and 201 (inclusive), and `random.sample(range(100, 201, 2), 5)` randomly chooses 5 numbers from this list.

Finally, the line `print(resp)` prints the list of 5 random numbers.