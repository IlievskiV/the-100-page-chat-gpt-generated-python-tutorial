# Exercise 91
Please write a program which accepts a string from console and print it in reverse order.

## Code
```python
s = input()
s = "".join(reversed(s))
print(s)
```

## ChatGPT Explanation
This code takes an input string from the user and reverses its characters. The `input()` function is used to get the string from the user. Then, the `reversed` function is used to reverse the order of characters in the string. 

Finally, the `join` function is used to join the reversed characters together into a new string, which is then printed to the console.