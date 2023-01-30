# Exercise 40
Write a program which accepts a string as input to print "Yes" if the string is "yes" or "YES" or "Yes", otherwise print "No".

## Code
```python
input = input("Enter string:")
output = "".join(
    ["Yes" if input == "yes" or input == "YES" or input == "Yes" else "No"]
)
print(str(output))
```

## ChatGPT Explanation
This code snippet prompts the user to enter a string and then assigns the input to a variable called `input`. 

It then uses a `join` method to join a list of strings together. The list is created using a list comprehension that checks if the input is equal to "yes", "YES", or "Yes", if it is it returns "Yes" otherwise it returns "No". 

The final result is then stored in the `output` variable and printed as a string. The output will be "Yes" if the user entered "yes", "YES", or "Yes" and "No" for any other input.