# Exercise 36
Define a function which can generate a list where the values are square of numbers between 1 and 20 (both included). Then the function needs to print all values except the first 5 elements in the list.


## Code
```python
def printList():
    lst = [i ** 2 for i in range(1, 21)]
    for i in range(5, 20):
        print(lst[i])

printList()
```

## ChatGPT Explanation
This code defines a function called `printList()`. Inside the function, it creates a list called `lst` that contains the squares of the numbers from 1 to 20. Then it uses a `for` loop to iterate through a range of numbers from 5 to 20 (not including 20), and for each iteration, it prints the element of the `lst` list at that index. 

So it will print the elements of the list that are at index 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, and 19. Essentially, it is printing the last 15 elements of the list.