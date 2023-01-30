# Exercise 98
Given 2 sets of integers, M and N, print their symmetric difference in ascending order. The term symmetric difference indicates those values that exist in either M or N but do not exist in both.

## Code
```python
n = int(input())
set1 = set(map(int, input().split()))

m = int(input())
set2 = set(map(int, input().split()))

ans = list(set1 ^ set2)
ans.sort()
for i in ans:
    print(i)
```

## ChatGPT Explanation

This code takes two sets of integers as input and finds the symmetric difference between them. The symmetric difference of two sets is defined as the set of elements that are in either of the sets, but not in their intersection.

1. The first input line `n` is the number of elements in set 1, and the next line is the elements of `set1`, separated by spaces. These elements are converted to integers using the `map` function and stored in `set1`.

2. The next two lines are similar, with `m` being the number of elements in `set2`, and the next line being the elements of `set 2`. These elements are stored in `set2`.

3. The symmetric difference between the two sets is found using the `^` operator, and the result is stored in the list `ans`.

4. The list `ans` is sorted and the elements are printed one by one.