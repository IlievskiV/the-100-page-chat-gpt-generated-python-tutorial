# Exercise 30
Define a function that can accept two strings as input and print the string with maximum length in console. If two strings have the same length, then the function should print all strings line by line.


## Code
```python
func = (
    lambda a, b: print(max((a, b), key=len))
    if len(a) != len(b)
    else print(a + "\n" + b)
)
```

## ChatGPT Explanation

This code defines a lambda function `func` that takes in two arguments `a` and `b`. 

The function then checks if the lengths of `a` and `b` are not equal. If they are not, it prints the argument with the larger length using the `max` function and the `len` key. If the lengths are equal, it prints both `a` and `b` on separate lines using string concatenation. Note that this function definition doesn't execute it. 

You would need to call the function by passing two parameters.