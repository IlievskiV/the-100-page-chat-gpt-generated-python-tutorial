# Exercise 35

Define a function which can generate a list where the values are square of numbers between 1 and 20 (both included). Then the function needs to print the last 5 elements in the list.

## Code
```python
def printList():
    lst = [i ** 2 for i in range(1, 21)]
    for i in range(19, 14, -1):
        print(lst[i])

printList()
```

## ChatGPT Explanation
This function creates a list of the squares of the numbers from 1 to 20 using a list comprehension. Then, it uses a `for` loop to iterate through the list in reverse order, starting from the 19th index and going to the 14th index (with a step of -1, to count backwards). For each iteration, the function prints the value of the corresponding element in the list. So it will print the squares of the numbers 15 to 20 in descending order.