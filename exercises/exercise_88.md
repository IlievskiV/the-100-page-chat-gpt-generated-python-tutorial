# Exercise 88
With a given list [12,24,35,24,88,120,155,88,120,155], write a program to print this list after removing all duplicate values with original order reserved.

## Code
```python
li = [12, 24, 35, 24, 88, 120, 155, 88, 120, 155]
for i in li:
    if li.count(i) > 1:
        li.remove(i)
print(li)
```

## ChatGPT Explanation
This code snippet creates a list of integers called `li` and then loops through each element `i` in the list. 

For each iteration of the loop, it checks if the count of `i` in the list is greater than 1. If the count is greater than 1, it removes the first occurrence of `i` from the list using the `remove` method.

Finally, it prints the updated list after all the duplicates have been removed.