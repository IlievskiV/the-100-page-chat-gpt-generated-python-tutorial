# Exercise 81
By using list comprehension, please write a program to print the list after removing numbers which are divisible by 5 and 7 in [12,24,35,70,88,120,155].

## Code
```python
li = [12, 24, 35, 70, 88, 120, 155]
li = [x for x in li if x % 35 != 0]
print(li)
```

## ChatGPT Explanation
The code defines a list of integers called `li`. Then, it uses a list comprehension to create a new list of integers, filtering out the elements of `li` that are divisible by 35.

The `if x % 35 != 0` part in the list comprehension checks whether `x` is not divisible by 35. If this condition is true, then `x` is added to the new list.

Finally, the code prints the new filtered list.