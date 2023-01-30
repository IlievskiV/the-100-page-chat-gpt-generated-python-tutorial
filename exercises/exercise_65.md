# Exercise 65
Please write assert statements to verify that every number in the list [2,4,6,8] is even.

## Code
```python
data = [2, 4, 5, 6]
for i in data:
    assert i % 2 == 0, "{} is not an even number".format(i)
```

## ChatGPT Explanation
This code is checking if each element in the list `data` is even or not. If the element is not even, it will raise an `AssertionError` with the message `"x is not an even number"`, where `x` is the current element in the iteration. 

The `assert` statement is used to check if a given condition is met, and if not, raise an exception. In this case, the condition being checked is if the element divided by 2 has a remainder of 0 (i.e. if it is even). If this condition is met for all elements in the list, the code will execute without raising any exceptions.