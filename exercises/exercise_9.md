# Exercise 9
Write a program that accepts sequence of lines as input and prints the lines after making all characters in the sentence capitalized.

## Code
```python
def user_input():
    while True:
        s = input()
        if not s:
            return
        yield s

for line in map(str.upper, user_input()):
    print(line)
```

## ChatGPT Explanation

This code defines a function `user_input()` that takes no arguments and continuously prompts the user for input until they provide an empty string (by just pressing enter). Each input string provided by the user is then passed to the `str.upper()` method to convert the string to uppercase and then passed to the `print()` function to print it out. The `map()` function applies `str.upper()` method to each input string.

The `while` loop in the function `user_input()` uses the `input()` function to continuously prompt the user for input and assigns the input string to the variable `s`. 

The `if not s:` line checks whether the input string is empty or not. If it is empty, the return statement is executed, which terminates the function and the loop stops. If the input string is not empty, it is passed to the yield statement, which returns the input string to the calling code and continues to execute the next iteration of the loop.

The `for` loop uses the `user_input()` function to get user input and the `map()` function to call the `str.upper()` method on each input string to convert it to uppercase and the `print()` function to print it out.