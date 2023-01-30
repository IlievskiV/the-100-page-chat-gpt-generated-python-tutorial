# Exercise 42
Write a program which can map() and filter() to make a list whose elements are square of even number in [1,2,3,4,5,6,7,8,9,10].

## Code
```python
def even(x):
    return x % 2 == 0


def squer(x):
    return x * x

li = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
li = map(
    squer, filter(even, li)
)  # first filters number by even number and the apply map() on the resultant elements
print(list(li))
```

## ChatGPT Explanation
The code defines two functions: `even(x)` and `square(x)`. The even function takes a single argument `x` and returns `True` if `x` is even and `False` otherwise. The square function takes a single argument `x` and returns `x` squared.

Then it creates a list of numbers called li. It then uses the `map()` function to apply the square function to each element in the list. But before applying the square function, it applies the `filter` function to the list, which filters out all the elements that are not even. 

So the final output will be the square of even numbers of the list.