# Exercise 54
Assuming that we have some email addresses in the "username@companyname.com" format, please write program to print the company name of a given email address. Both user names and company names are composed of letters only.


## Code
```python
import re

email = "john@google.com elise@python.com"
pattern = "\w+@(\w+).com"
ans = re.findall(pattern, email)
print(ans)
```

## ChatGPT Explanation
The code imports the `re` (regular expression) module. Then it defines a string `email` that contains two email addresses.

A regular expression pattern pattern is then defined to match words `(\w+)` before the `@` symbol, followed by another word `(\w+)` and `.com`.

The `re.findall` function is called, passing in the `pattern` and `email` strings. The function returns a list of all the matches found in the `email` string and it is assigned to the variable `ans`.

Finally, `ans` is printed, which would output: `['google', 'python']`.