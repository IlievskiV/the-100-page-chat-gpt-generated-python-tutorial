# Exercise 27

Define a function that can convert a integer into a string and print it in console.

## Code
```python
conv = lambda x: str(x)
n = conv(10)
print(n)
print(type(n))  # checks the type of the variable
```

## ChatGPT Explanation

This code defines a lambda function named `conv`, which takes in a single argument `x` and returns the string representation of that argument.

It then assigns the value of the function applied to the integer 10 to a variable `n`. It then prints out the value of `n` and it's data type using the `print` and `type` function respectively. It will output:

```
10
<class 'str'>
```