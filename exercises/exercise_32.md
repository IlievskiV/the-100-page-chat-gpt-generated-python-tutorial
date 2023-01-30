# Exercise 32
Define a function which can generate a dictionary where the keys are numbers between 1 and 20 (both included) and the values are square of keys. The function should just print the keys only.


## Code
```python
def printDict():
    dict = {i: i ** 2 for i in range(1, 21)}
    print(dict.keys())  # print keys of a dictionary

printDict()
```

## ChatGPT Explanation
This code defines a function called `printDict()`. Inside the function, it creates a dictionary called `dict` with keys being integers from 1 to 20, and values being the square of the corresponding key. 

Then it calls the `keys()` method on the `dict` object, which returns a view object of all the keys in the dictionary, and prints it. When the function is called, it will print all the keys in the dictionary (1, 2, 3, 4, ..., 20) without values.