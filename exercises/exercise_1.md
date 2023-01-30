# Exercise 1

Write a program which will find all such numbers which are divisible by 7 but are not a multiple of 5, between 2000 and 3200 (both included).The numbers obtained should be printed in a comma-separated sequence on a single line.

## Code

``` python
for i in range(2000, 3201):
    if i % 7 == 0 and i % 5 != 0:
        print(i, end=",")
print("\b")
```

## ChatGPT Explanation

This code snippet outputs all the numbers between 2000 and 3200 (inclusive) that are divisible by 7 but not divisible by 5.

The `for` loop iterates over the range of numbers from 2000 to 3200 and the `if` statement inside the loop checks if the current number `i` is divisible by 7 but not divisible by 5. If the condition is true, then the current number `i` is printed, followed by a comma. 

Finally, the `\b` at the end of the code removes the last comma.