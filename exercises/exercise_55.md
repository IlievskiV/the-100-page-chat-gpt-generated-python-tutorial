# Exercise 55
Write a program which accepts a sequence of words separated by whitespace as input to print the words composed of digits only.

## Code
```python
email = input().split()
ans = [word for word in email if word.isdigit()]  # using list comprehension method
print(ans)
```

## ChatGPT Explanation
This code takes a list of words as input and splits it into separate words. Then it uses a list comprehension to extract all the words that are numbers. Finally, it prints the resulting list of numbers.