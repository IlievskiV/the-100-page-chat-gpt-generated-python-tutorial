# Exercise 96
You are given a string S and width W. Your task is to wrap the string into a paragraph of width.

If the following string is given as input to the program:
- ABCDEFGHIJKLIMNOQRSTUVWXYZ 4

Then, the output of the program should be:
- ABCD EFGH IJKL IMNO QRST UVWX YZ

## Code
```python
import textwrap

string = input()
width = int(input())

print(textwrap.fill(string, width))
```

## ChatGPT Explanation
The code snippet is using the `textwrap` module to wrap a given text string into multiple lines.

The user inputs the text string and the width (number of characters per line) they want to wrap the text into.

The code then calls the `fill` method from the `textwrap` module and passes in the text string and the desired width as arguments. This method returns the text string, wrapped into multiple lines so that no line exceeds the width specified.

Finally, the wrapped text is printed to the console.