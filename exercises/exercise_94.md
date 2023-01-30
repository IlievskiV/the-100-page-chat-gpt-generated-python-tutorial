# Exercise 94
Write a program to solve a classic ancient Chinese puzzle: We count 35 heads and 94 legs among the chickens and rabbits in a farm. How many rabbits and how many chickens do we have?

## Code
```python
def solve(numheads, numlegs):
    ns = "No solutions!"
    for i in range(numheads + 1):
        j = numheads - i
        if 2 * i + 4 * j == numlegs:
            return i, j
    return ns, ns

numheads = 35
numlegs = 94
solutions = solve(numheads, numlegs)
print(solutions)
```

## ChatGPT Explanation
The code defines a function named `solve` that takes two parameters `numheads` and `numlegs`. It then uses a `for` loop to iterate over a range of values starting from 0 to the value of `numheads + 1`. Within the loop, it calculates the value of `j` by subtracting the current value of `i` from `numheads`. Then, it checks if the result of the expression `2 * i + 4 * j` is equal to `numlegs`. If it is, it returns a tuple of values `i` and `j`.

If the loop completes and no solutions are found, the function returns a tuple `ns, ns` which contains the string `"No solutions!"`.

Finally, the code sets `numheads` to 35 and `numlegs` to 94, then calls the `solve` function passing these values. The returned solution is then printed.