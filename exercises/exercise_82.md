# Exercise 82
By using list comprehension, please write a program to print the list after removing the 0th, 2nd, 4th,6th numbers in [12,24,35,70,88,120,155].

## Code
```python
li = [12, 24, 35, 70, 88, 120, 155]
li = [li[i] for i in range(len(li)) if i % 2 != 0]
print(li)
```

## ChatGPT Explanation
This code snippet uses Python to create a list `li` of numbers, and then creates a new list `li` with only the elements located at odd indices of the original list `li`.

It starts by defining a list `li` of 7 integers.

Then, it creates a new list `li` using a list comprehension. The list comprehension includes all elements located at odd indices (indexes 1, 3, 5, etc.) of the original list `li`.

Finally, the new list `li` is printed to the console.