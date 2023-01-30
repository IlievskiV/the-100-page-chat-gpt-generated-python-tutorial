# Exercise 60
Write a program to compute:
`f(n) = f(n - 1) + 100, n>0`
with a given n input by console (n>0).

## Code
```python
def f(n):
    if n == 0:
        return 0
    return f(n - 1) + 100

n = int(input())
print(f(n))
```

## ChatGPT Explanation
The following code is a recursive function in Python that calculates the sum of the series `100 + 200 + 300 + ... + 100 * n`where `n` is the input argument.

The function `f(n)` takes an integer `n` as input. If `n` is 0, it returns 0. Otherwise, it calls itself with the argument `n-1` and adds 100 to the result. This process repeats until the base case of `n=0` is reached, and then the final result is returned up the call stack.

The code also takes a user input `n`, converts it to an integer, and passes it as an argument to the `f` function. The result of the `f` function is then printed.