# Exercise 83
By using list comprehension, please write a program to print the list after removing the 2nd - 4th numbers in [12,24,35,70,88,120,155].

## Code
```python
li = [12, 24, 35, 70, 88, 120, 155]
li = [li[i] for i in range(len(li)) if i < 3 or 4 < i]
print(li)
```

## ChatGPT Explanation
This code snippet is written in Python and it defines a list called `li` which contains 7 numbers.

The next line of code creates a new list called `li` which contains elements of the original list `li` based on the conditions specified in a list comprehension.

A list comprehension is a concise way of creating a new list from an existing one.

The condition specified in this list comprehension is `if i < 3 or 4 < i`, which means the elements will be selected if the index of the element (`i`) is less than 3 or greater than 4.

Finally, the new list is printed using the `print()` function.