# Exercise 43
Write a program which can filter() to make a list whose elements are even number between 1 and 20 (both included).


## Code
```python
def even(x):
    return x % 2 == 0

evenNumbers = filter(even, range(1, 21))
print(list(evenNumbers))
```

## ChatGPT Explanation
The code defines a function called `even(x)` that takes in a parameter `x` and returns `True` if `x` is even, and `False` if `x` is odd. 

Then, it uses the `filter()` function to filter out all the even numbers in the range of 1 to 21 and assigns the resulting filter object to the variable `evenNumbers`. 

Finally, it converts the filter object into a list and prints it. So the output will be a list of all even numbers between 1 and 21.