# Exercise 78
Please write a program to shuffle and print the list [3,6,7,8].

## Code
```python
import random

lst = [3, 6, 7, 8]
random.shuffle(lst)
print(lst)
```

## ChatGPT Explanation

This code is in the Python programming language. It makes use of the `random` module which provides a set of functions for generating pseudo-random numbers.

The code defines a list called `lst` that contains the values [3, 6, 7, 8].

Then, the function `shuffle` from the `random` module is used to shuffle the items in the list `lst`. The `shuffle` function randomly reorders the items in the list.

Finally, the shuffled list is printed using the `print` statement.