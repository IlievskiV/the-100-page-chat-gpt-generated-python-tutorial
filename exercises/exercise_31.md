# Exercise 31
Define a function which can print a dictionary where the keys are numbers between 1 and 20 (both included) and the values are square of keys.

## Code
```python
def printDict():
    dict = {i: i ** 2 for i in range(1, 21)}
    print(dict)

printDict()
```

## ChatGPT Explanation
This code defines a function `printDict()`. When called, the function creates a dictionary, `dict`, with keys being numbers from 1 to 20, and values being the square of the corresponding key. It then prints the dictionary to the console.