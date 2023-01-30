# Exercise 84
By using list comprehension, please write a program generate a 3*5*8 3D array whose each element is 0

## Code
```python
array = [[[0 for col in range(8)] for col in range(5)] for row in range(3)]
```

## ChatGPT Explanation

The code creates a 3-dimensional list in Python, also called an array. This array has 3 layers. The first layer has 3 rows. The second layer has 5 columns. The third layer has 8 columns. Each value in the 3rd layer is set to zero.

In other words, the code creates a 3x5x8 matrix filled with zeros. The matrix has 3 pages, with each page having 5 rows and 8 columns, making a total of 3 x 5 x 8 = 120 zeros in the array.