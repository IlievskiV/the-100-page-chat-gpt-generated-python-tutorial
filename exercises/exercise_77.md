# Exercise 77
Please write a program to print the running time of execution of "1+1" for 100 times.

## Code
```python
import time

before = time.time()
for i in range(100):
    x = 1 + 1
after = time.time()
execution_time = after - before
print(execution_time)
```

## ChatGPT Explanation
The code is measuring the execution time of a simple operation. It's using the `time` module in Python which provides various time-related functions.

At the start of the code, the current time is recorded by `before = time.time()`.

Then, the code runs a for loop 100 times where a simple operation `x = 1 + 1` is performed.

At the end of the loop, the current time is recorded again by `after = time.time()`.

Finally, the execution time is calculated by subtracting `before` from `after` and stored in the variable `execution_time`. The execution time is then printed using `print(execution_time)`. This shows how much time it took to run the simple operation 100 times.