# Exercise 12

Write a program, which will find all such numbers between 1000 and 3000 (both included) such that each digit of the number is an even number.The numbers obtained should be printed in a comma-separated sequence on a single line.

## Code

```python
lst = [str(i) for i in range(1000, 3001)]
lst = list(
    filter(lambda i: all(ord(j) % 2 == 0 for j in i), lst)
)  # using lambda to define function inside filter function
print(",".join(lst))
```

## ChatGPT Explanation

This code generates a list of numbers between 1000 and 3000 and filters out the numbers that have any odd-numbered digits in them.

The first line of code uses a list comprehension to generate a list of numbers between 1000 and 3000 and converts them to strings.

The next line of code uses the `filter()` function to filter out the numbers that have any odd-numbered digits in them. `filter()` function applies the lambda function to each element in the list, the lambda function takes one argument `i`, and for each digit `j` in `i` , it checks whether the ASCII value of `j` is even using the `ord()` function and the modulus operator `%` . If all digits are even, the lambda function returns `True`, and the number is kept in the list, otherwise it filters out the number.

Finally, the `join()` method is used to join the filtered list of numbers into a string of comma-separated numbers and then the string is printed out.