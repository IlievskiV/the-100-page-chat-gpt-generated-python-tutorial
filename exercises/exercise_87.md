# Exercise 87
With two given lists [1,3,6,78,35,55] and [12,24,35,24,88,120,155], write a program to make a list whose elements are intersection of the above given lists.

## Code
```python
list1 = [1, 3, 6, 78, 35, 55]
list2 = [12, 24, 35, 24, 88, 120, 155]
set1 = set(list1)
set2 = set(list2)
intersection = set.intersection(set1, set2)
print(intersection)
```

## ChatGPT Explanation
The code defines two lists, `list1` and `list2` with some values. Then, it creates two sets `set1` and `set2` from these two lists respectively.

The `intersection` variable is assigned the result of the intersection of `set1` and `set2` using the `intersection` method of the `set` class. This method returns a set that contains all the elements that are present in both `set1` and `set2`.

Finally, the code prints the `intersection` variable which contains the result of the intersection of `set1` and `set2`.