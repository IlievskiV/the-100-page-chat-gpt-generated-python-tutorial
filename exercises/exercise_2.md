# Exercise 2
Write a program which can compute the factorial of a given numbers.The results should be printed in a comma-separated sequence on a single line.Suppose the following input is supplied to the program: 8 Then, the output should be:40320

## Code
```python
n = int(input())
fact = 1
for i in range(1, n + 1):
    fact = fact * i
print(fact)
```

## ChatGPT Explanation

This code snippet is a simple program that calculates the factorial of a given number.

The first line of code is getting an input from the user and assigns it to the variable `n`. The `int` function is used to convert the input to an integer.

The next line creates a variable called `fact` and assigns it the value of 1.

The following `for` loop starts with the variable `i` set to 1, and it will run as long as `i` is less than or equal to `n + 1`, and `i` will increment by 1 after each iteration.

In each iteration, the value of `fact` is multiplied by `i` and the result is stored in `fact` again, so on each iteration `fact` will be updated with the new value.

After the loop has finished, the final value of fact is printed using the `print()` function.