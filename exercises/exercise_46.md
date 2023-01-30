# Exercise 46
Define a class named American and its subclass NewYorker.

## Code
```python
class American:
    pass

class NewYorker(American):
    pass

american = American()
newyorker = NewYorker()

print(american)
print(newyorker)
```

## ChatGPT Explanation

The code defines two classes `American` and `NewYorker` in Python. The `American` class is an empty class which doesn't have any attributes or methods. The `NewYorker` class is a subclass of `American` class.

In the code, two objects `american` and `newyorker` are created. The first object `american` is an instance of the `American` class, while the second object `newyorker` is an instance of the `NewYorker` class.

When the `print` statement is executed, the object `american` returns the memory location of the `american` object. The object `newyorker` returns the memory location of the `newyorker` object.

The output will be:
```
<__main__.American object at 0x...>
<__main__.NewYorker object at 0x...>
```