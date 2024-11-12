List Comprehensions


Traditional approach:

```python

numbers = []
for i in range(5):
    numbers.append(i * i)

```
List comprehension:

```python

numbers = [i * i for i in range(5)]

```

Examples:
```python
evens = [x for x in range(10) if x % 2 == 0]
print(evens)  # Output: [0, 2, 4, 6, 8]


```


```python
squares = [x * x for x in range(6)]
print(squares)  # Output: [0, 1, 4, 9, 16, 25]


```

 List Comprehensions with Conditions

```python
evens = [x for x in range(10) if x % 2 == 0]
print(evens)  # Output: [0, 2, 4, 6, 8]

```
Example (multiple conditions):

```python
multiples_of_three = [x for x in range(30) if x % 3 == 0 and x % 2 == 0]
print(multiples_of_three)  # Output: [0, 6, 12, 18, 24]


```
Nested List Comprehensions:

```python
matrix = [[j for j in range(3)] for i in range(3)]
print(matrix)
# Output: [[0, 1, 2], [0, 1, 2], [0, 1, 2]]


```
Practical Example: Filtering and Transforming Lists

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8]
squares_of_evens = [x * x for x in numbers if x % 2 == 0]
print(squares_of_evens)  # Output: [4, 16, 36, 64]


```
Exercise: List Comprehensions


Instructions:

Use the string "Hello World!".
Write a list comprehension that filters out the uppercase letters.

```python

string = "Hello World!"
uppercase_letters = [char for char in string if char.isupper()]
print(uppercase_letters)  # Output: ['H', 'W']

```
