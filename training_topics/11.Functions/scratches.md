What are Functions?

```python
def greet():
    print("Hello, world!")
```

Defining and Calling Functions


```python
# Defining a function
def say_hello():
    print("Hello!")

# Calling a function
say_hello()  # Output: Hello!
```

Function Parameters and Arguments

```python
# Function with parameters
def greet_user(name):
    print(f"Hello, {name}!")

# Calling the function with an argument
greet_user("Alice")  # Output: Hello, Alice!
```


```python
def add_numbers(a, b):
    return a + b

result = add_numbers(3, 4)
print(result)  # Output: 7
```

Return Values

```python
# Function that returns a value
def square(number):
    return number * number

# Storing the returned value in a variable
result = square(5)
print(result)  # Output: 25

```

Practical Examples

```python
#Example 1: Temperature Conversion
def celsius_to_fahrenheit(celsius):
    return (celsius * 9/5) + 32

print(celsius_to_fahrenheit(25))  # Output: 77.0

```


```python
#Example 2: Checking Even or Odd

def is_even(number):
    if number % 2 == 0:
        return True
    else:
        return False

print(is_even(4))  # Output: True
print(is_even(7))  # Output: False

```


```python
#Example 3: Finding the Maximum of Three Numbers


def find_max(a, b, c):
    return max(a, b, c)

print(find_max(5, 10, 3))  # Output: 10


```

Exercises


Exercise 1: Simple Greeting Function
```python
# Write a function that takes a name as input and prints a personalized greeting.
def greet(name):
    # Your code here
    print(f"Hello, {name}!")
    
# Test the function
greet("John")

```

Exercise 2: Calculate the Area of a Circle

```python
# Write a function that calculates the area of a circle given its radius.
import math

def area_of_circle(radius):
    # Your code here
    return math.pi * radius ** 2

# Test the function
print(area_of_circle(5))  # Output: 78.53981633974483

```

Exercise 3: Find the Sum of a List


```python
# Write a function that takes a list of numbers and returns their sum.
def sum_of_list(numbers):
    # Your code here
    total = 0
    for num in numbers:
        total += num
    return total

# Test the function
print(sum_of_list([1, 2, 3, 4]))  # Output: 10

```
