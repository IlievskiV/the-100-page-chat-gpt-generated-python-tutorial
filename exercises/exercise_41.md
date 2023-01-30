# Exercise 41
Write a program which can map() to make a list whose elements are square of elements in [1,2,3,4,5,6,7,8,9,10].

## Code
```python
li = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
squaredNumbers = map(lambda x: x ** 2, li)  # returns map type object data
print(list(squaredNumbers))  # converting the object into list

```

## ChatGPT Explanation
The code above uses the `map()` function to apply the lambda function `lambda x: x ** 2` to each element in the list `li`. 

The lambda function takes one argument `x` and returns the square of `x`. The `map()` function returns a map object, which is an iterator over the results of applying the lambda function to each element in the list. The `list()` function is then used to convert the map object into a list, so that the squared numbers can be printed using the `print()` function. 

The output will be the list of squared numbers of the elements in the original list.
