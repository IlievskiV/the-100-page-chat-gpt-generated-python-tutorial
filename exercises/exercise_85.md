# Exercise 85
By using list comprehension, please write a program to print the list after removing the 0th, 4th, 5th numbers in [12,24,35,70,88,120,155].

## Code
```python
li = [12, 24, 35, 70, 88, 120, 155]
li = [li[i] for i in range(len(li)) if i not in (0, 4, 5)]
print(li)
```

## ChatGPT Explanation

This code defines a list of numbers named `li`. It then creates a new list named `li` which consists of elements from the original `li` list where the index is not equal to 0, 4, and 5.

The new `li` is constructed using a list comprehension. A list comprehension is a concise way to create a new list in Python.
The syntax is:

```python
new_list = [expression for item in iterable if condition]
```

In this code, expression is `li[i]`, iterable is `range(len(li))`, and `condition` is `i not in (0, 4, 5)`. This expression generates a new list with elements from the `li` list where the index is not 0, 4, or 5. Finally, the code prints the new `li`.