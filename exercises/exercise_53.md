# Exercise 53
Assuming that we have some email addresses in the "username@companyname.com" format, please write program to print the user name of a given email address. Both user names and company names are composed of letters only.

## Code
```python
import re

email = "john@google.com elise@python.com"
pattern = "(\w+)@\w+.com"
ans = re.findall(pattern, email)
print(ans)
```

## ChatGPT Explanation

The given code uses the `re` module in Python to find all occurrences of a specific pattern in a string. The pattern being searched for is defined as `"(\w+)@\w+.com"` and it represents an email address format.

The `findall` method of the `re` module is used to search the string `email` and return all occurrences of the pattern defined in pattern. The result is stored in the `ans` variable and finally, the result is printed using the `print` statement.

The output of the code will be `['john', 'elise']`, which are the substrings that match the pattern.