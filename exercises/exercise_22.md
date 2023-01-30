# Exercise 22

Write a program to compute the frequency of the words from the input. The output should output after sorting the key alphanumerically.


## Code
```python
from pprint import pprint

p = input().split()
pprint({i: p.count(i) for i in p})
```


## ChatGPT Explanation

This code snippet in Python is used for counting the occurrences of each element in a given list and printing the results in a dictionary format. 

The input is taken as a string of elements separated by a space, which is then split into a list of elements using the `split` method. The `pprint` module is imported to format the output as a dictionary. A dictionary comprehension is used to iterate over the list of elements and count the occurrences of each element. The resulting dictionary is then printed using the `pprint` function.