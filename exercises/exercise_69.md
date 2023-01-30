# Exercise 69
Please generate a random float where the value is between 5 and 95 using Python module.

## Code
```python
import random

rand_num = random.uniform(5, 95)
print(rand_num)
```

## ChatGPT Explanation

The code generates a random floating-point number between 5 and 95.

The first line `import random` is used to import the `random` module in Python, which provides functions for generating random numbers.

The second line `rand_num = random.uniform(5, 95)` generates a random floating-point number between 5 and 95 (including 5 but not including 95) and assigns it to the variable `rand_num`.

Finally, the line `print(rand_num)` prints the generated random number.