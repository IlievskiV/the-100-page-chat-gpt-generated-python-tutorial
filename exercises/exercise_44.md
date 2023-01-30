# Exercise 44
Write a program which can map() to make a list whose elements are square of numbers between 1 and 20 (both included).

## Code
```python
def sqr(x):
    return x * x

squaredNumbers = list(map(sqr, range(1, 21)))
print(squaredNumbers)
```

## ChatGPT Explanation
In this code snippet, we are defining a function `sqr` that takes in a single argument `x` and returns the square of `x` by multiplying `x` with itself.

Next, we use the `map` function to apply the `sqr` function to every element in the range 1 to 21 (exclusive). This creates a map object, which is a lazy evaluation of the function applied to each element in the range.

To obtain the list of the squared numbers, we use the `list` function to convert the map object into a list and store it in the variable `squaredNumbers`.

Finally, we print the `squaredNumbers` list to see the output, which is the list of squares of numbers from 1 to 20.