# Exercise 18

A website requires the users to input username and password to register. Write a program to check the validity of password input by users. Following are the criteria for checking the password:

- At least 1 letter between [a-z]
- At least 1 number between [0-9]
- At least 1 letter between [A-Z]
- At least 1 character from [$#@]
- Minimum length of transaction password: 6
- Maximum length of transaction password: 12

Your program should accept a sequence of comma separated passwords and will check them according to the above criteria. Passwords that match the criteria are to be printed, each separated by a comma.

## Code

```python
def is_low(x):  # Returns True  if the string has a lowercase
    for i in x:
        if "a" <= i and i <= "z":
            return True
    return False

def is_up(x):  # Returns True  if the string has a uppercase
    for i in x:
        if "A" <= i and i <= "Z":
            return True
    return False

def is_num(x):  # Returns True  if the string has a numeric digit
    for i in x:
        if "0" <= i and i <= "9":
            return True
    return False

def is_other(x):  # Returns True if the string has any "$#@"
    for i in x:
        if i == "$" or i == "#" or i == "@":
            return True
    return False

s = input().split(",")
lst = []

for i in s:
    length = len(i)
    if (
        6 <= length
        and length <= 12
        and is_low(i)
        and is_up(i)
        and is_num(i)
        and is_other(i)
    ):  # Checks if all the requirments are fulfilled
        lst.append(i)

print(",".join(lst))
```

## ChatGPT Explanation

This script takes input of a string of comma-separated values, and checks each value against certain conditions. The conditions are:

1. The length of the string is between 6 and 12 characters
2. The string contains at least one lowercase letter
3. The string contains at least one uppercase letter
4. The string contains at least one numeric digit
5. The string contains at least one of the special characters "$#@".

The script uses 4 separate functions (`is_low`, `is_up`, `is_num`, `is_other`) to check if each string meets each of these requirements.

If a value meets all these conditions, it is added to a list. Finally, the script prints all the values in the list, joined by commas.

The function `is_low(x)` checks if the input string `x` has any lowercase letters by iterating through each character in the string and checking if it falls within the range of lowercase letters. It returns `True` if at least one lowercase letter is found, and `False` otherwise.

The function `is_up(x)` returns `True` if the input string `x` contains at least one uppercase letter, and `False` otherwise. It iterates through each character in the input string, and checks if it is within the range of uppercase letters using the comparison operator `<=`. If it finds an uppercase letter, it immediately returns `True`. If it reaches the end of the input string without finding an uppercase letter, it returns `False`.

The function `is_num(x)` takes in a single argument `x` which is a string. The function then uses a `for` loop to iterate through each character in the string `x`. Within the `for` loop, there is an `if` statement that checks if the current character being iterated through is a numeric digit (i.e. between 0 and 9). If the current character is a numeric digit, the function immediately returns `True`. If the for loop completes without finding a numeric digit, the function returns `False` at the end. In other words, this function checks if the input string contains any numeric digits, and returns `True` if it does and `False` if it does not.


The function `is_other(x)` takes in a single input, `x`. The function then iterates through each character in the input `x` using a for loop. Inside the loop, the function checks if the current character is equal to any of the special characters `$`, `#`, or `@`. If any of these characters are present in the input, the function immediately returns `True`. If the loop completes without finding any of these characters, the function returns `False` indicating that none of the special characters were found in the input.