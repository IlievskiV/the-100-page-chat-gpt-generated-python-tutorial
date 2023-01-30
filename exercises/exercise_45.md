# Exercise 45
Define a class named American which has a static method called printNationality.

## Code
```python
class American:
    @staticmethod
    def printNationality():
        print("I am American")

american = American()
american.printNationality()
American.printNationality()
```

## ChatGPT Explanation

The code defines a class `American` in Python. The class has a static method called `printNationality()`. This method simply prints the string `"I am American"`.

A object `american` is created from the `American` class. The object american invokes the `printNationality()` method using the object instance `american.printNationality()`.

The class `American` directly invokes the static method `printNationality()` by calling `American.printNationality()`.

Both of these method invocations produce the same output "I am American".