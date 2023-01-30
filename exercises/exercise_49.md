# Exercise 49
Define a class named Shape and its subclass Square. The Square class has an init function which takes a length as argument. Both classes have a area function which can print the area of the shape where Shape's area is 0 by default.

## Code
```python
class Shape:
    def __init__(self):
        pass

    def area(self):
        return 0

class Square(Shape):
    def __init__(self, length=0):
        Shape.__init__(self)
        self.length = length

    def area(self):
        return self.length * self.length


Asqr = Square(5)
print(Asqr.area())

print(Square().area())
```

## ChatGPT Explanation

The code defines a class `Shape` that has an `__init__` method which takes no arguments, and an `area` method that returns `0`. 

It also defines a class `Square` that inherits from the `Shape` class. The `Square` class has an `__init__` method that takes an optional argument `length` and initializes the `length` attribute of the object. The `Square` class also overrides the `area` method of the `Shape` class to return the area of a square, which is calculated as the square of its length.

The code then creates an object `Asqr` of the `Square` class with the length 5 and prints its area by calling the `area` method on the object. The code also creates another object of the `Square` class with no arguments and prints its area, which is 0 because the length was not specified.