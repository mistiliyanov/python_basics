Lambda Functions

Traditional approach vs. lambda function:

```python

# Standard function
def square(x):
    return x * x

# Lambda function
square = lambda x: x * x

```

```python

add = lambda x, y: x + y
print(add(2, 3))  # Output: 5

```
Using Lambda Functions with Built-In Functions

```python

numbers = [1, 2, 3, 4]
squares = list(map(lambda x: x * x, numbers))
print(squares)  # Output: [1, 4, 9, 16]


```

Using filter with lambda

```python

numbers = [1, 2, 3, 4, 5, 6]
evens = list(filter(lambda x: x % 2 == 0, numbers))
print(evens)  # Output: [2, 4, 6]


```
Using sorted with lambda


```python

names = ["Alice", "Bob", "Charlie", "Dave"]
sorted_names = sorted(names, key=lambda x: len(x))
print(sorted_names)  # Output: ['Bob', 'Dave', 'Alice', 'Charlie']


```

Practical Examples

Sorting a List of Tuples

```python

students = [("Alice", 24), ("Bob", 20), ("Charlie", 23)]
sorted_students = sorted(students, key=lambda x: x[1])
print(sorted_students)
# Output: [('Bob', 20), ('Charlie', 23), ('Alice', 24)]


```

Using Lambdas in List Comprehensions

```python

numbers = [1, 2, 3, 4]
doubled = [(lambda x: x * 2)(x) for x in numbers]
print(doubled)  # Output: [2, 4, 6, 8]


```

Creating Lambda Functions

```python

is_multiple_of_three = lambda x: x % 3 == 0
print(is_multiple_of_three(9))   # Output: True
print(is_multiple_of_three(10))  # Output: False


```
Limitations of Lambda Functions:

### Lambda functions are concise, but they have a few limitations:

* Single Expression Only: Lambda functions can only contain a single expression, which means no complex logic or multiple statements.

* Limited Readability: Overusing lambda functions in complex expressions can make code harder to read.

* No Annotations: Lambda functions don’t support type annotations, which can be a drawback for more complex functions.

* In summary, use lambda functions for short, simple tasks, and stick to def functions for anything more complex.

```python

```

Best Practices for Using Lambda Functions

Let’s go over a few best practices for working with lambda functions:

* Keep it Simple: Only use lambdas for simple operations. If it’s more complex, use a def function.
* Avoid Overuse: Use lambdas when you need a short function temporarily, such as in map or sorted.
* Focus on Readability: If a lambda function makes code less readable, consider using a named function instead.

Example of clear vs. unclear lambda

```python
# Clear
evens = list(filter(lambda x: x % 2 == 0, range(10)))

# Unclear
nested = lambda x: lambda y: x * y

```


```python

```
