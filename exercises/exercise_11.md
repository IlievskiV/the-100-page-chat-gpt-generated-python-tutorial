# Exercise 11

Write a program which accepts a sequence of comma separated 4 digit binary numbers as its input and then check whether they are divisible by 5 or not. The numbers that are divisible by 5 are to be printed in a comma separated sequence.

## Code

```python
data = input().split(",")
data = list(
    filter(lambda i: int(i, 2) % 5 == 0, data)
)  # lambda is an operator that helps to write function of one line
print(",".join(data))
```

## ChatGPT Explanation

This code takes a string of comma-separated binary numbers as input, filters out the numbers that are not divisible by 5 when converted to decimal, and then prints the remaining numbers as a comma-separated string.

The first line of code uses the `input()` function to get user input, which is expected to be a string of comma-separated binary numbers. It then uses the `split()` method to convert the input string into a list of binary numbers by splitting it at each comma.

The next line of code uses the `filter()` function to filter out the binary numbers that are not divisible by 5 when converted to decimal. `filter()` function applies the lambda function to each element in the list, the lambda function takes one argument `i`, converts it to decimal using `int(i, 2)` and check whether it's divisible by 5 or not, if it's true it keeps the element otherwise it filters out the element.

Finally, the `join()` method is used to join the filtered list of binary numbers into a string of comma-separated binary numbers and then the string is printed out.