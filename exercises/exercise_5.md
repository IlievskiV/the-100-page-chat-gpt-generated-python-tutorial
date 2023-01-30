# Exercise 5

Define a class which has at least two methods:
- `getString`: to get a string from console input
- `printString`: to print the string in upper case.

## Code
```python
class IOstring:
	def __init__(self):
        pass

    def get_string(self):
        self.s = input()

    def print_string(self):
        print(self.s.upper())


xx = IOstring()
xx.get_string()
xx.print_string()
```

## ChatGPT Explanation

This code snippet is a simple program that defines a class called `IOstring`, which has two methods: `get_string()` and `print_string()`.

The `__init__` method is the constructor of the class, it is called when an object of this class is created and does not have any specific functionality in this case, it just pass.

The `get_string()` method prompts the user to input a string and assigns it to the variable `s` as an attribute of the class.

The `print_string()` method then takes the value stored in the `s` attribute, converts it to uppercase using the `upper()` method, and prints it out.

The last three lines of code are creating an object of the IOstring class called `xx`, calling the `get_string()` method on it to set the value of the `s` attribute, and then calling the `print_string()` method to print the value of `s` in uppercase.