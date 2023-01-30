# Exercise 38
With a given tuple (1,2,3,4,5,6,7,8,9,10), write a program to print the first half values in one line and the last half values in one line.

## Code
```python
tup = (1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
lt = int(len(tup) / 2)
print(tup[:lt], tup[lt:])
```

## ChatGPT Explanation

The code creates a tuple `tup` containing the numbers 1 to 10. Then it creates a variable `lt` that is the integer division of the length of the tuple by 2. 

Finally, it prints out the first half of the tuple by slicing it from the start to the index of `lt` and the second half of the tuple by slicing it from the index of lt to the end. 

The final output would be `(1, 2, 3, 4, 5)` `(6, 7, 8, 9, 10)`.