# Exercise 90
Please write a program which count and print the numbers of each character in a string input by console.

## Code
```python
import string

s = input()
for letter in string.ascii_lowercase:
    cnt = s.count(letter)
    if cnt > 0:
        print("{},{}".format(letter, cnt))
```

## ChatGPT Explanation

This code is a program that takes in a string as input from the user and then counts the number of occurrences of each letter in the string (case-insensitive). 

It uses the `string` module's `ascii_lowercase` constant to get a list of all lowercase letters in the alphabet. The program loops over each letter in `ascii_lowercase`, and for each letter, it counts the number of occurrences of that letter in the input string `s` using the `count` method. If the count of a letter is greater than 0, the program prints the letter and its count in the format `"{},{}"`.