# Exercise 39
Write a program to generate and print another tuple whose values are even numbers in the given tuple (1,2,3,4,5,6,7,8,9,10).

## Code
```python
tpl = (1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
tpl1 = tuple(i for i in tpl if i % 2 == 0)
print(tpl1)
```

## ChatGPT Explanation
This code creates a tuple called `tpl` that contains the integers 1 through 10. It then creates a new tuple called `tpl1` that contains only the even numbers from `tpl` using a list comprehension. 

It iterates over each element in `tpl` and checks if it is divisible by 2 using the modulo operator. If it is, it adds it to the new tuple `tpl1`. 

Finally, it prints out the new tuple `tpl1`, which should contain the numbers 2, 4, 6, 8, and 10.