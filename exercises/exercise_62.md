# Exercise 62
The Fibonacci Sequence is computed based on the following formula:
```
f(0)=0,
f(1)=1,
f(n) = f(n - 1) + f(n - 2), n > 1
```
Please write a program to compute the value of f(n) with a given n input by console and prints all the values all along.

## Code
```python
def f(n):
    if n < 2:
        fibo[n] = n
        return fibo[n]
    fibo[n] = f(n - 1) + f(n - 2)
    return fibo[n]

n = int(input())
fibo = [0] * (n + 1)  # initialize a list of size (n+1)
f(n)  # call once and it will set value to fibo[0-n]
fibo = [str(i) for i in fibo]  # converting integer data to string type
ans = ",".join(fibo)  # joining all string element of fibo with ',' character
print(ans)
```

## ChatGPT Explanation
The code above calculates the first n terms of the Fibonacci sequence using a recursive function `f`.

The function takes an argument `n` and checks if it is less than 2. If it is, it stores n in the `fibo` list and returns `n`.

Otherwise, it calculates the n-th term of the sequence by calling the function with `n-1` and `n-2` as arguments, adds the results and stores it in the `fibo` list. The function returns the n-th term.

The function is called with the input value of n and the fibo list is initialized with 0's. The function is called to calculate the first `n` terms of the sequence and the results are stored in the fibo list.

Finally, the list is converted to a string with each element separated by a comma and the result is printed.