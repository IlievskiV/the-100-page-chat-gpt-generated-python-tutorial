# Exercise 72
Please write a program to generate a list with 5 random numbers between 100 and 200 inclusive.

## Code
```python
import random

resp = random.sample(range(100, 201), 5)
print(resp)
```

## ChatGPT Explanation
This code snippet is written in Python and uses the `random` module to generate a list of 5 random numbers within the range of 100 to 200 (inclusive).

First, we import the `random` module, which provides a suite of functions for generating pseudo-random numbers.

Next, we use the `random.sample` method to generate a list of 5 random numbers within the range of 100 to 200. The `random.sample` method takes two arguments: the first argument is the range of numbers to choose from (in this case, it's `range(100, 201)`), and the second argument is the number of items to choose from that range (in this case, it's 5).

Finally, we use the `print` function to output the list of 5 randomly generated numbers.