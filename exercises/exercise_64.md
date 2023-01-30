# Exercise 64
Please write a program using generator to print the numbers which can be divisible by 5 and 7 between 0 and n in comma separated form while n is input by console.

## Code
```python
def generate(n):
    for i in range(n + 1):
        if (
            i % 35 == 0
        ):  # 5*7 = 35, if a number is divisible by a & b then it is also divisible by a*b
            yield i

n = int(input())
resp = [str(i) for i in generate(n)]
print(",".join(resp))
```

## ChatGPT Explanation
The following code snippet defines a function called `generate` that takes an integer `n` as input. The function uses the `range` function to generate a range of numbers from 0 to `n` and uses a for loop to iterate through this range.

The `for` loop checks if the number `i` is divisible by 35, if it is divisible, it is added to the generator using the `yield` keyword. This allows us to generate a sequence of numbers that are divisible by 35.

Finally, the list comprehension `resp` takes the numbers generated from the generator and converts them into a list of strings. The list is then joined using the `join` method and separated by a comma. The final result is then printed to the console.