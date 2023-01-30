# Exercise 17

Write a program that computes the net amount of a bank account based a transaction log from console input. The transaction log format is shown as following:

```
D 100
W 200
```

D means deposit while W means withdrawal.

## Code

```python
lines = []
while True:
    loopInput = input()
    if loopInput == "done":
        break
    else:
        lines.append(loopInput)

lst = list(int(i[2:]) if i[0] == "D" else -int(i[2:]) for i in lines)
print(sum(lst))
```

## ChatGPT Explanation

This code snippet first creates an empty list called `lines`. 

It then enters a `while` loop that continues until the user inputs `"done"`. For each iteration of the loop, the script takes in user input and checks if it is `"done"`. If it is not, it appends the input to the `lines` list. 

Once the loop breaks, the script creates a new list called `lst` using list comprehension. It iterates through each element of `lines` and checks if the first character of the element is `"D"`. If it is, it adds the element as is to the new list, otherwise it adds the element as a negative number. 

Finally, the script calculates the sum of the elements in the `lst` list and prints it.