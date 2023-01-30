## Exercise 25

Define a class, which have a class parameter and have a same instance parameter.

### Code
```python
class Car:
    name = "Car"
    def __init__(self, name=None):
        self.name = name

honda = Car("Honda")
print(f"{Car.name} name is {honda.name}")

toyota = Car()
toyota.name = "Toyota"
print(f"{Car.name} name is {toyota.name}")
```

### ChatGPT Explanation

This code defines a class called `Car` with a class variable `name` which is set to "Car" by default. When creating a new object of the `Car` class, you can pass in a custom name as an argument, otherwise it will use the default "Car" value.

The first instance of the class is created and assigned to the variable `honda`. The class variable name is overridden with the value "Honda" that was passed in during the object's creation. Then a message is printed, displaying the class variable's value of "Car" and the object variable's value of "Honda".

The second instance of the class is created and assigned to the variable `toyota`. In this case, the name of the object is not passed during the object creation, so the default value of "Car" is used. Later, the object variable's value is overridden with "Toyota" and a message is printed, displaying the class variable's value of "Car" and the object variable's value of "Toyota".