# Exercise 33
Define a function which can generate and print a list where the values are square of numbers between 1 and 20 (both included).

## Code
```python
def printList():
    lst = [i ** 2 for i in range(1, 21)]
    print(lst)

printList()
```

## ChatGPT Explanation

This code defines a function called `printList()` that creates a list of the squares of the numbers from 1 to 20 (inclusive). It then prints the list to the console.

When the function is called (by the last line `printList()`), it will execute the instructions inside it and print the list of the squares of the numbers from 1 to 20 to the console.