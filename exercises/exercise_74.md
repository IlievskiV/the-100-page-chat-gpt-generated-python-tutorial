# Exercise 74
Please write a program to randomly generate a list with 5 numbers, which are divisible by 5 and 7 , between 1 and 1000 inclusive.

## Code
```python
import random

lst = [i for i in range(1, 1001) if i % 35 == 0]
resp = random.sample(lst, 5)
print(resp)

```

## ChatGPT Explanation

This code snippet imports the `random` module in Python, which provides functions to generate random numbers.

The first line defines a list called `lst` which contains all the numbers from 1 to 1000 that are divisible by 35. This is done using a list comprehension.

The second line uses the `random.sample` function from the `random` module to generate 5 random numbers from the list `lst`. This function takes two arguments, the first is the list from which the random samples should be selected, and the second is the number of samples to select.

Finally, the last line prints the result of the `resp` variable, which contains the 5 random numbers selected from the `lst` list.