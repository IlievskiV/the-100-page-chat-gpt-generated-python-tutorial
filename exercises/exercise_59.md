# Exercise 59
Write a program to compute 1/2+2/3+3/4+...+n/n+1 with a given n input by console (n>0).

## Code
```python
n = int(input())
sum = 0
for i in range(1, n + 1):
    sum += i / (i + 1)
print(round(sum, 2))  # rounded to 2 decimal point
```

## ChatGPT Explanation

The code snippet computes and prints the sum of a series. The series formula is defined as follows:

`sum = (1/2) + (2/3) + (3/4) + ... + (n/(n + 1))`

The input `n` is expected to be a positive integer and determines the number of terms in the series. The code uses a `for` loop to iterate through the range 1 to `n + 1` and calculates each term of the series by dividing `i` by `(i + 1)` where `i` is the current iteration value. Finally, the sum of all terms is calculated and rounded to 2 decimal places using the `round` function. The result is then printed.