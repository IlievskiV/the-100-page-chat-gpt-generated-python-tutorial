# Exercise 15

Write a program that computes the value of `a+aa+aaa+aaaa` with a given digit as the value of a.

## Code
```python
a = input()
total, tmp = 0, str()  # initialing an integer and empty string

for i in range(4):
    tmp += a  # concatenating 'a' to 'tmp'
    total += int(tmp)  # converting string type to integer type

print(total)
```

## ChatGPT Explanation

This code takes an input, and then assigns it to a variable `a`.

It then initializes two variables, `total` and `tmp`, with the values of 0 and empty string respectively.

The code then uses a `for` loop that iterates 4 times. In each iteration, it concatenates the variable `a` to the variable `tmp` and then converts it to an integer and adds it to the variable `total`.

At the end, it prints the total.