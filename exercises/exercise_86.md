# Exercise 86
By using list comprehension, please write a program to print the list after removing the value 24 in [12,24,35,24,88,120,155].

## Code
```python
li = [12, 24, 35, 24, 88, 120, 155]
li.remove(24)  # this will remove only the first occurrence of 24
print(li)
```

## ChatGPT Explanation
This code defines a list named `li` with some values. Then, it removes the first occurrence of the value 24 from the list using the `remove()` method. Finally, it prints the resulting list.