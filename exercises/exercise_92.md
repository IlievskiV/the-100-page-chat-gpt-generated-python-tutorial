# Exercise 92
Please write a program which accepts a string from console and print the characters that have even indexes.

## Code
```python
s = "H1e2l3l4o5w6o7r8l9d"
s = [s[i] for i in range(len(s)) if i % 2 == 0]
print("".join(s))
```

## ChatGPT Explanation
The given code takes a string `s` and creates a new list of characters by picking characters at even-indexed positions in the input string `s`. 

The final output is a concatenation of all the characters in the new list, represented as a string. The result is printed on the console.