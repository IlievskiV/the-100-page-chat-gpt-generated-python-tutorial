# Exercise 19

You are required to write a program to sort the (name, age, score) tuples by ascending order where name is string, age and score are numbers. The tuples are input by console. The sort criteria is:

1. Sort based on name
2. Then sort based on age
3. Then sort by score


## Code
```python
lst = []
while True:
    s = input().split(",")
    if not s[0]:  # breaks for blank input
        break
    lst.append(tuple(s))

lst.sort(
    key=lambda x: (x[0], x[1], x[2])
)  # here key is defined by lambda and the data is sorted by element priority 0>1>2 in accending order
print(lst)
```

## ChatGPT Explanation

This code snippet is a Python program that prompts the user for input of strings separated by commas. 

It creates an empty list called `lst` and enters a `while` loop. Within the `while` loop, it takes user input, splits it into a list of strings by the commas, and assigns it to the variable `s`. If the first element of `s` is blank, the loop breaks. Otherwise, it appends a tuple of the elements of `s` to `lst`. 

After the loop, the program sorts `lst` by the first, second, and third elements of each tuple, and then prints `lst`.