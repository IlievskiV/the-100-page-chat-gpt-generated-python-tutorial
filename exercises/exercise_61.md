# Exercise 61
The Fibonacci Sequence is computed based on the following formula:
```
f(0)=0,
f(1)=1,
f(n) = f(n - 1) + f(n - 2), n > 1
```
Please write a program to compute the value of f(n) with a given n input by console.

## Code
```python
def f(n):
    if n < 2:
        return n
    return f(n - 1) + f(n - 2)

n = int(input())
print(f(n))
```

## ChatGPT Explanation

This code implements the recursive function `f(n)`, which returns the n-th number in the Fibonacci sequence. The Fibonacci sequence is a sequence of numbers where each number is the sum of the two preceding numbers. In this case, the sequence starts with 0 and 1, so the first two numbers in the sequence are 0 and 1.

The function first checks if `n` is less than 2, and if so, it returns `n`. This serves as the base case for the recursion. If `n` is greater than or equal to 2, the function calls itself twice, each time with an argument that is one less than the current value of `n`. The two calls to `f(n - 1)` and `f(n - 2)` represent the two preceding numbers in the sequence, and the sum of these two calls gives the next number in the sequence. This process continues until `n` becomes less than 2, at which point the base case is reached and the recursion stops.

Finally, the code takes an input `n` from the user, and passes it as an argument to the function `f(n)`. The function returns the n-th number in the Fibonacci sequence, which is printed to the screen.