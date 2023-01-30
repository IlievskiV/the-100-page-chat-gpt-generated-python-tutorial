# Exercise 34
Define a function which can generate a list where the values are square of numbers between 1 and 20 (both included). Then the function needs to print the first 5 elements in the list.

## Code
```python
func = lambda: ([i ** 2 for i in range(1, 21)][:5])
print(*(func()), sep="\n")
```

## ChatGPT Explanation
This code defines a lambda function `func` that returns a list of the first 5 squares of the integers from 1 to 20. 

The lambda function is immediately called and the result is unpacked and passed as separate arguments to the `print` function, which then separates the items in the list with newlines and prints them. The output will be a list of the first five square of numbers 1 to 20.