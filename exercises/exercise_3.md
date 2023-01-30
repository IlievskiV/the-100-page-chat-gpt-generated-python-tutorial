# Exercise 3

With a given integral number n, write a program to generate a dictionary that contains `(i, i x i)` such that is an integral number between 1 and `n` (both included). and then the program should print the dictionary. Suppose the following input is supplied to the program: 8

## Code
```python
n = int(input())
ans = {}
for i in range(1, n + 1):
	ans[i] = i * i
print(ans)
```


## ChatGPT Explanation

This code snippet is a simple program that creates a dictionary where the keys are the integers from 1 to `n`, and the values are the square of the corresponding key.

The first line of code is getting an input from the user and assigns it to the variable `n`. The int function is used to convert the input to an integer.

The next line creates an empty dictionary called `ans`.

The following for loop starts with the variable `i` set to 1, and it will run as long as `i` is less than or equal to `n + 1`, and `i` will increment by 1 after each iteration.

In each iteration, the `i` is used as key in the dictionary `ans` and the value is calculated as `i * i` and assigned to that key. After the loop has finished, the final dictionary `ans` is printed using the `print()` function.