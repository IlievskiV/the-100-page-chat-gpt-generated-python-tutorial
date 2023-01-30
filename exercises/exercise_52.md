# Exercise 52
Define a custom exception class which takes a string message as attribute.

## Code
```python
class CustomException(Exception):
    """Exception raised for custom purpose

    Attributes:
        message -- explanation of the error
    """

    def __init__(self, message):
        self.message = message

num = int(input())
try:
    if num < 10:
        raise CustomException("Input is less than 10")
    elif num > 10:
        raise CustomException("Input is grater than 10")
except CustomException as ce:
    print("The error raised: " + ce.message)
```

## ChatGPT Explanation
The code defines a custom exception class called `CustomException` that inherits from the built-in `Exception` class. The custom exception class takes in a message as an argument and sets it as an attribute.

The code then takes in a number from the user, converts it to an integer, and stores it in the `num` variable. The code then uses a `try-except` block to handle the custom exception.

If `num` is less than 10, the code raises the custom exception with the message `"Input is less than 10"`. If `num` is greater than 10, the code raises the custom exception with the message `"Input is greater than 10"`.

In the except block, the code prints the message attribute of the custom exception, with the message `"The error raised: "` concatenated to the front.