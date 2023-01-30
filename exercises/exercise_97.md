# Exercise 97
You are given a date. Your task is to find what the day is on that date.

## Code
```python
import calendar

month, day, year = map(int, input().split())
dayId = calendar.weekday(year, month, day)
print(calendar.day_name[dayId].upper())

```

## ChatGPT Explanation
This code is using the `calendar` module in Python to find the day of the week for a given date.

First, it takes three inputs from the user: `month`, `day`, and `year`. These three inputs are combined into a single string, then separated and converted into integers using the `map` function and the `int` function.

Next, the `calendar.weekday` function is used to determine the weekday for the given date. This function takes three arguments: the year, the month, and the day. The result is an integer representing the day of the week, where Monday is 0 and Sunday is 6.

Finally, the `calendar.day_name` array is used to convert the integer representation of the day of the week into a string, and the `upper` function is used to convert the string to uppercase. The resulting string is then printed.