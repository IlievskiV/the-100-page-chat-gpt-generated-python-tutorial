# Exercise 71
Please write a program to output a random number, which is divisible by 5 and 7, between 10 and 150 inclusive using random module and list comprehension.

## Code
```python

import random

resp = [i for i in range(10, 151) if i % 35 == 0]
print(random.choice(resp))
```

## ChatGPT Explanation

The code imports the `random` module in Python, which provides functions for generating pseudo-random numbers. 

Then, it defines a list called `resp` using a list comprehension that generates a list of numbers from 10 to 150 (inclusive) that are divisible by 35 (i.e., have a remainder of 0 when divided by 35). 

Finally, the code prints a random element from this list using the `random.choice` function, which returns a randomly selected element from a given sequence (in this case, the `resp` list).