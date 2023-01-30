# Exercise 14

Write a program that accepts a sentence and calculate the number of upper case letters and lower case letters.

## Code
```Python
string = input("Enter the sentense")
upper = 0
lower = 0
for x in string:
    if x.isupper() == True:
        upper += 1
    if x.islower() == True:
        lower += 1

print("UPPER CASE: ", upper)
print("LOWER CASE: ", lower)
```

## ChatGPT Explanation

This code takes an input string, and then it iterates over each character in the string.

For each character, it checks if the character is uppercase using the `isupper()` method. If it is uppercase, the variable upper is incremented by 1.

Then, it checks if the character is lowercase using the `islower()` method. If it is lowercase, the variable lower is incremented by 1.

Finally, it prints the count of uppercase and lowercase characters in the input string.