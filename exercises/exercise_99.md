# Exercise 99
You are given words. Some words may repeat. For each word, output its number of occurrences. The output order should correspond with the input order of appearance of the word. See the sample input/output for clarification.

If the following string is given as input to the program:
- `4 bcdef abcdefg bcde bcdef`

Then, the output of the program should be:
- `3 2 1 1`

## Code
```python
n = int(input())

word_list = []
word_dict = {}

for i in range(n):
    word = input()
    if word not in word_dict:
        word_list.append(word)
    word_dict[word] = word_dict.get(word, 0) + 1

print(len(word_list))
for word in word_list:
    print(word_dict[word], end=" ")
```

## ChatGPT Explanation

This code takes in an integer `n` as input which represents the number of words to be entered. Then it takes `n` words as input and stores them in a list `word_list`. It also creates a dictionary `word_dict` where the key is a word and the value is the frequency of that word in the input words.

It then checks if a word is not already present in the dictionary, if yes, it appends the word to the list `word_list`. It then increments the value of the word in the dictionary by 1.

In the end, it prints the length of the list `word_list` and the frequency of each word in `word_dict` separated by a space.