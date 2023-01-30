# Exercise 63
Please write a program using generator to print the even numbers between 0 and n in comma separated form while n is input by console.

## Code
```python
def EvenGenerator(n):
    i = 0
    while i <= n:
        if i % 2 == 0:
            yield i
        i += 1

n = int(raw_input())
values = []
for i in EvenGenerator(n):
    values.append(str(i))

print ",".join(values)
```

## ChatGPT Explanation

The following code generates a list of even numbers up to a given number `n`. This is achieved using a generator function `EvenGenerator(n)`. The generator function `EvenGenerator(n)` generates even numbers up to `n` using a `while` loop.

The `yield` statement is used in the generator function to return each even number. This allows the generator to pause its execution after each iteration and return the current value of `i`. This way, we can generate a series of even numbers without having to store them all in memory.

The generator function is called with the input `n` and the generated even numbers are stored in the list `values`. The `values` list is then converted to a string separated by commas using the `join` method and printed as the final result.