# Exercise 100
You are given a string.Your task is to count the frequency of letters of the string and print the letters in descending order of frequency. 

If the following string is given as input to the program:
- `aabbbccde` 

Then, the output of the program should be:
- `b 3 a 2 c 2 d 1 e 1`

## Code
```python
s = list(input())

dict_count_ = {k: s.count(k) for k in s}
list_of_tuples = [(k, v) for k, v in dict_count_.items()]
list_of_tuples.sort(key=lambda x: x[1], reverse=True)

for item in list_of_tuples:
    print(item[0], item[1])
```

## ChatGPT Explanation
The following code in Python takes an input string, `s`, and performs the following actions:

1. Creates a dictionary, `dict_count_`, where each character in the string is a key and its value is the count of that character in the string.

2. Creates a list of tuples, `list_of_tuples`, where each tuple consists of a character and its count.

3. Sorts the list of tuples in descending order of the count of characters.

4. Prints the character and its count for each tuple in the sorted list.