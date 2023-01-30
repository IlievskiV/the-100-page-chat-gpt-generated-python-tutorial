# Exercise 28
Define a function that can receive two integer numbers in string form and compute their sum and then print it in console.

## Code
```python
sum = lambda s1, s2: int(s1) + int(s2)
print(sum("10", "45"))  # 55
```

## ChatGPT Explanation
This code defines a lambda function called `sum`, which takes in two parameters `s1` and `s2` and converts them from strings to integers using the `int()` function.

Then it performs the sum of the integers and returns the result. Then, the code calls the `sum` function with the arguments "10" and "45" and prints the result, which is 55.