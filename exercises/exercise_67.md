# Exercise 67
Please write a binary search function which searches an item in a sorted list. The function should return the index of element to be searched in the list.

## Code
```python
def binary_search_Ascending(array, target):
    lower = 0
    upper = len(array)
    print("Array Length:", upper)
    while lower < upper:
        x = (lower + upper) // 2
        print("Middle Value:", x)
        value = array[x]
        if target == value:
            return x
        elif target > value:
            lower = x
        elif target < value:
            upper = x

Array = [1, 5, 8, 10, 12, 13, 55, 66, 73, 78, 82, 85, 88, 99]
print("The Value Found at Index:", binary_search_Ascending(Array, 82))
```

## ChatGPT Explanation
The code performs a binary search algorithm in an ascending sorted array to find the index of a target value.

The function `binary_search_Ascending` takes two arguments, `array` and `target`. It first initializes two variables, `lower` and `upper`, to be the start and end of the array, respectively. The `while` loop runs until `lower` becomes greater than or equal to `upper`. In each iteration, `x` is calculated as the middle value of the current subarray defined by `lower` and `upper`, and the value of the array at that index is stored in `value`.

Then, the `target` value is compared with the `middle` value, if they are equal, the index `x` is returned as the answer. If the `target` value is greater than the `middle` value, lower is updated to be equal to `x` so that the next search will be in the upper half of the array. If the target value is less than the middle value, `upper` is updated to be equal to `x`, so that the next search will be in the lower half of the array.

The `print` statements are used for debugging purposes to see the intermediate values of `x` and the length of the array.

The code then calls the function with an example array and target value and prints the index at which the target value is found.