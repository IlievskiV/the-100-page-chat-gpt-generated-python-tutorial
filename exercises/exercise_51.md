# Exercise 51
Write a function to compute 5/0 and use try/except to catch the exceptions.

## Code
```python
def divide():
    return 5 / 0

try:
    divide()
except ZeroDivisionError as ze:
    print("Why on earth you are dividing a number by ZERO!!")
except:
    print("Any other exception")
```

## ChatGPT Explanation
The code block implements a simple `try-except` block to handle exceptions raised during the execution of the `divide` function.

The `divide` function returns the result of dividing 5 by 0, which will raise a `ZeroDivisionError` exception.

In the `try` block, we call the `divide` function, and in the following `except` block, we handle the `ZeroDivisionError` exception by printing a custom error message: `"Why on earth you are dividing a number by ZERO!!"`.

In case any other exception is raised, we catch it in another `except` block and print a different message: `"Any other exception"`.

This way, if an exception is raised during the execution of the `divide` function, it will be caught and handled, and the program will not crash.