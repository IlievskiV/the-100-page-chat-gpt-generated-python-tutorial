# Exercise 37
Define a function which can generate and print a tuple where the value are square of numbers between 1 and 20 (both included).

## Code
```python
def square_of_numbers():
    return tuple(i ** 2 for i in range(1, 21))

print(square_of_numbers())

```

## ChatGPT Explanation
This code defines a function `square_of_numbers()` that creates and returns a tuple containing the squares of numbers from 1 to 20 (inclusive). 

The function uses a `generator` expression to create the tuple, which is more memory efficient than creating a list and then converting it to a tuple. The function doesn't take any parameters. When the function is called and the tuple is returned, it is then printed to the console.