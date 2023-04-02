# Python map, filter and reduce

Python comes with a set of built-in functions that are used for manipulating iterables such as lists, tuples, and sets. Among these are the [map, filter, and reduce functions in python](https://www.programdoc.com/python/map-filter-reduce).

A [lambda function is a type of anonymous function in Python](https://www.programdoc.com/python/lambda) that can be declared using a single line of expression. These functions can be passed as arguments to other functions, making it easier to write expressions in a single statement and to understand the code.

The `map()` function takes a function and an iterable as arguments. It then applies the function to each value in the iterable and returns an iterator containing the processed values. Here's an example that squares the values of a list using `map()`:

```py
numbers = [1, 2, 3, 4, 5]
squared_numbers = list(map(lambda i: i ** 2, numbers))
print(squared_numbers) 
# Output: [1, 4, 9, 16, 25]
``` 

The `filter()` function is similar to `map()`, but with one difference. It returns an iterator containing only the elements from a sequence for which a given function returns `True`. Here's an example that filters even numbers from a list using `filter()`:

```py
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_numbers = list(filter(lambda i: i % 2 == 0, numbers))
print(even_numbers)
# Output: [2, 4, 6, 8, 10]
``` 

The `reduce()` function takes a function and an iterable as arguments. It then applies the function to the first two values in the iterable and passes the result along with the next value to the function again. This process continues until there is only one value left, which is then returned. Here's an example that calculates the product of a list of numbers using `reduce()`:

```py
from functools import reduce
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
product = reduce(lambda i, j: i * j, numbers)
print(product)
# Output: 3628800
``` 
