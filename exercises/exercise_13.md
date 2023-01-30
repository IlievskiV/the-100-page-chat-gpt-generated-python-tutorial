# Exercise 13

Write a program that accepts a sentence and calculate the number of letters and digits.

## Code
```python
word = input()
letter, digit = 0, 0

for i in word:
    if i.isalpha():  # returns True if alphabet
        letter += 1
    elif i.isnumeric():  # returns True if numeric
        digit += 1
print(
    f"LETTERS {letter}\n{digits}"
)  # two different types of formating method is shown in both solution
```

## ChatGPT Explanation

This code takes an input string, and then it iterates over each character in the string.

For each character, it checks if the character is an alphabet using the `isalpha()` method. If it is an alphabet, the variable letter is incremented by 1.

Then, it checks if the character is a digit using the `isnumeric()` method. If it is a digit, the variable digit is incremented by 1.

Finally, it prints the count of letters and digits in the input string. `f"LETTERS {letter}\n{digits}"` is used to format the output string where letter and digit are the variables that contain the count of letters and digits respectively in the input word.