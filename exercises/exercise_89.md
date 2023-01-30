# Exercise 89
Define a class Person and its two child classes: Male and Female. All classes have a method "getGender" which can print "Male" for Male class and "Female" for Female class.

## Code
```python
class Person(object):
    def getGender(self):
        return "Unknown"


class Male(Person):
    def getGender(self):
        return "Male"


class Female(Person):
    def getGender(self):
        return "Female"


aMale = Male()
aFemale = Female()
print(aMale.getGender())
print(aFemale.getGender())
```

## ChatGPT Explanation
The code creates a Python class called `Person` with a method `getGender` that returns the string `"Unknown"`. 

The class `Male` is a subclass of the `Person` class, and it overrides the `getGender` method to return the string `"Male"`. Similarly, the class `Female` is a subclass of the `Person` class and it overrides the `getGender` method to return the string `"Female"`.

Next, the code creates two objects, `aMale` and `aFemale`, from the classes `Male` and `Female`, respectively. Finally, the code prints the result of calling the getGender method on each object. This will print `"Male"` and `"Female"`.