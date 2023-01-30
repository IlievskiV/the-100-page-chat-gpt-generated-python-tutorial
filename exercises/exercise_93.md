# Exercise 93
Please write a program which prints all permutations of [1,2,3]

## Code
```python
import itertools
print(list(itertools.permutations([1, 2, 3])))
```

## ChatGPT Explanation
This code uses the `itertools` module in Python to generate all possible permutations of a given list `[1, 2, 3]`.

The `permutations` function from the `itertools` module takes a list as input and returns an iterable object containing all possible arrangements (permutations) of the elements in that list.

In this code, the permutations are computed for the list `[1, 2, 3]`, and the result is then converted to a list using the `list` function. 

The final output of the code will be a list of all possible permutations of the list `[1, 2, 3]`.