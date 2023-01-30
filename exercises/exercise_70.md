# Exercise 70
Please write a program to output a random even number between 0 and 10 inclusive using random module and list comprehension.

## Code
```python
import random

resp = [i for i in range(0, 11, 2)]
print(random.choice(resp))

```

## ChatGPT Explanation
The code imports the `random` module in Python, which provides a suite of functions to generate pseudo-random numbers.

Then, a list `resp` is created using list comprehension, with the numbers from 0 to 10 with a step of 2.

Finally, the `random.choice` method is used to select a random element from the list `resp`. The selected random element is then printed to the console. This code will output a random even number between 0 and 10.