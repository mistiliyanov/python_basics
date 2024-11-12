Map, Filter, Reduce


Map:
```python
numbers = [1, 2, 3, 4]
squares = list(map(lambda x: x * x, numbers))
print(squares)  # Output: [1, 4, 9, 16]

```

Filter:
```python
numbers = [1, 2, 3, 4, 5, 6]
evens = list(filter(lambda x: x % 2 == 0, numbers))
print(evens)  # Output: [2, 4, 6]

```


Reduce:
```python
from functools import reduce
numbers = [1, 2, 3, 4]
product = reduce(lambda x, y: x * y, numbers)
print(product)  # Output: 24

```

Practical Example – Combining map, filter, and reduce

Let’s combine these functions in a practical example. Imagine we want to process a list of numbers to achieve the following:

1. Double each number.
2. Filter out numbers greater than 10.
3. Calculate the sum of the remaining numbers.

```python
from functools import reduce
numbers = [1, 3, 5, 7, 9]

# Step 1: Double each number
doubled = list(map(lambda x: x * 2, numbers))

# Step 2: Filter out numbers greater than 10
filtered = list(filter(lambda x: x <= 10, doubled))

# Step 3: Sum the remaining numbers
result = reduce(lambda x, y: x + y, filtered)

print(result)  # Output: 18

```

Exercise: Using Map, Filter, and Reduce

```python
from functools import reduce
numbers = [3, 5, 9, 12, 15, 18]

# Step 1: Triple each number
tripled = list(map(lambda x: x * 3, numbers))

# Step 2: Filter numbers divisible by 3
divisible_by_three = list(filter(lambda x: x % 3 == 0, tripled))

# Step 3: Find the maximum
max_number = reduce(lambda x, y: x if x > y else y, divisible_by_three)

print(max_number)  # Output should be 54

```
```python

```
