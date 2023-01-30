# Exercise 95
Given the participants' score sheet for your University Sports Day, you are required to find the runner-up score. You are given scores. Store them in a list and find the score of the runner-up.

If the following string is given as input to the program:
- 5 2 3 6 6 5

Then, the output of the program should be:
- 5

## Code
```python
arr = map(int, input().split())
arr = list(set(arr))
arr.sort()
print(arr[-2])
```

## ChatGPT Explanation
The code first takes an input from the user of a list of integers separated by spaces. The input is then passed to the `map` function which converts the strings into integers and returns a `map` object.

Next, the `map` object is converted into a list using the `list` function, and duplicates are removed by converting the list into a set and then back into a list.

Finally, the list is sorted in ascending order and the second last element is printed which is the second largest element in the list.