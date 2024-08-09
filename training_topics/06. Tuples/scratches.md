Tuples
What are Tuples?
```python
coordinates = (10.0, 20.0)
user_info = ("Alice", 30, "Engineer")
mixed_tuple = (1, "hello", 3.14, True)
```

Creating and Using Tuples

```python
# Creating tuples
empty_tuple = ()
single_element_tuple = (42,)
coordinates = (10.0, 20.0)

# Accessing elements by index
x = coordinates[0]
y = coordinates[1]
print("x coordinate:", x)  # Output: 10.0
print("y coordinate:", y)  # Output: 20.0

# Unpacking tuples
x, y = coordinates
print("Unpacked x:", x)  # Output: 10.0
print("Unpacked y:", y)  # Output: 20.0

```

Tuple Operations

```python
# Concatenation
tuple1 = (1, 2, 3)
tuple2 = (4, 5, 6)
combined_tuple = tuple1 + tuple2
print("Concatenation:", combined_tuple)  # Output: (1, 2, 3, 4, 5, 6)

# Repetition
repeated_tuple = tuple1 * 2
print("Repetition:", repeated_tuple)  # Output: (1, 2, 3, 1, 2, 3)

# Membership testing
is_in_tuple = 2 in tuple1
print("Is 2 in tuple1?", is_in_tuple)  # Output: True

```

Tuple Methods

```python
numbers = (1, 2, 3, 2, 4, 2)

# Count occurrences of an item
count_of_twos = numbers.count(2)
print("Count of 2s:", count_of_twos)  # Output: 3

# Find the index of an item
index_of_three = numbers.index(3)
print("Index of 3:", index_of_three)  # Output: 2

```


Practical Examples

Example 1: Returning Multiple Values from a Function

```python
def get_min_max(numbers):
    return min(numbers), max(numbers)

result = get_min_max([10, 20, 5, 40])
print("Min and Max:", result)  # Output: (5, 40)
```

Example 2: Swapping Values

```python
a = 10
b = 20
a, b = b, a
print("a:", a)  # Output: 20
print("b:", b)  # Output: 10
```

Example 3: Storing Coordinates

```python
Copy code
# Store multiple points as tuples in a list
points = [(1, 2), (3, 4), (5, 6)]
for point in points:
    print(f"Point: {point}")
```


Exercises

Exercise 1: Create and Use a Tuple

```python
# Create a tuple of three favorite movies
favorite_movies = ("The Matrix", "Inception", "Interstellar")

# Access and print the first and last movie in the tuple
first_movie = favorite_movies[0]
last_movie = favorite_movies[-1]
print("First movie:", first_movie)
print("Last movie:", last_movie)
```

Exercise 2: Unpacking a Tuple

```python
# Given a tuple with personal information
person_info = ("Alice", 30, "Engineer")

# Unpack the tuple into variables and print them
name, age, profession = person_info
print("Name:", name)
print("Age:", age)
print("Profession:", profession)
```