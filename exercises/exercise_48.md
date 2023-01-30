# Exercise 48
Define a class named Rectangle which can be constructed by a length and width. The Rectangle class has a method which can compute the area.

## Code
```python

class Rectangle:
    def __init__(self, l, w):
        self.length = l
        self.width = w

    def area(self):
        return self.length * self.width

rect = Rectangle(2, 4)
print(rect.area())
```

## ChatGPT Explanation

This code defines a class `Rectangle` in Python. The class has a constructor method `__init__` which initializes two instance variables `length` and `width` with the values passed as parameters when a `Rectangle` object is created. The class also has a method `area` which calculates and returns the area of the rectangle by multiplying the `length` and `width` of the object.

Finally, the code creates an instance of the `Rectangle` class and assigns it to the variable `rect`. The area of the rectangle is then printed by calling the `area` method on the rect object. The output of the code will be `8`.