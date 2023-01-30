# Exercise 80
Please write a program to print the list after removing even numbers in [5,6,77,45,22,12,24].

## Code
```python
li = [5, 6, 77, 45, 22, 12, 24]
lst = list(filter(lambda n: n % 2 != 0, li))
print(lst)
```

## ChatGPT Explanation
This is a Python code snippet that uses the `filter` method and `lambda` function to extract the odd numbers from a list.

The list `li` is initialized with a set of integers. The `filter` method and `lambda` function are used to extract only the odd numbers from the list. 

The `filter` method takes a function and a list as arguments. The `lambda` function is an anonymous function that takes an argument n and returns `True` if `n` is not divisible by 2, and `False` otherwise. The `filter` method then applies the `lambda` function to each element of the `li` list and returns a new list containing only the elements for which the function returns `True`. This new list is stored in the `lst` variable.

Finally, the resulting list is printed using the `print` function.