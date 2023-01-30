# Exercise 47
Define a class named Circle which can be constructed by a radius. The Circle class has a method which can compute the area.

## Code
```python
class Circle:
    def __init__(self, r):
        self.radius = r

    def area(self):
        return 3.1416 * (self.radius ** 2)

circle = Circle(5)
print(circle.area())
```

## ChatGPT Explanation

The code defines a class `Circle` with a constructor `__init__` method that takes a radius `r` as input and sets it as an instance variable `radius` of the object. The class also has a method `area` which calculates and returns the area of the circle using the formula `3.1416 * (self.radius ** 2)`.

Finally, an object `circle` of class `Circle` is created with radius 5 and its area is calculated by calling `circle.area()`. The result of the area calculation is then printed.