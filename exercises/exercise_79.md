# Exercise 79
Please write a program to generate all sentences where subject is in ["I", "You"] and verb is in ["Play", "Love"] and the object is in ["Hockey","Football"].

## Code
```python
subjects = ["I", "You"]
verbs = ["Play", "Love"]
objects = ["Hockey", "Football"]

for sub in subjects:
    for verb in verbs:
        for obj in objects:
            print("{} {} {}".format(sub, verb, obj))
```

## ChatGPT Explanation

The following code snippet in Python generates all possible combinations of a sentence using elements from three different lists: `subjects`, `verbs`, and `objects`.

The `subjects` list contains the words "I" and "You". The `verbs` list contains the words "Play" and "Love". The `objects` list contains the words "Hockey" and "Football".

The code uses a nested loop, with each outer loop iterating through each element in one of the lists (`subjects`, `verbs`, `objects`). The inner loop then iterates through the elements of the other two lists, combining each subject-verb-object combination and printing the resulting sentence.

For example, the first combination would be "I Play Hockey". The code will generate a total of (2 * 2 * 2 =) 8 combinations of sentences in total.