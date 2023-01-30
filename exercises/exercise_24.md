# Exercise 24
Please write a program to print some Python built-in functions documents, such as `abs()`, `int()`, `raw_input()`. And add document for your own function.

## Code
```python

def pow(n, p):
    """
    param n: This is any integer number
    param p: This is power over n
    return:  n to the power p = n^p
    """
    return n ** p

print(pow(3, 4))
print(pow.__doc__)
```

## ChatGPT Explanation

This is a Python function definition for a function called `pow` that takes in two parameters, `n` and `p`. 

The function calculates and returns the result of raising the value of `n` to the power of `p` (n to the power of `p = n^p`). The function also has a `docstring` that describes the purpose and parameters of the function.

The last two lines of the code snippet are calling the `pow` function with the values 3 and 4 as arguments, which will return 3^4 = 81 and also prints the `docstring` of the function.