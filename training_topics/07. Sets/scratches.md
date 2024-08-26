What are Sets?

```python
# Creating a set
fruits = {"apple", "banana", "cherry"}
numbers = {1, 2, 3, 4, 5}

```

Creating and Using Sets

```python
# Creating a set with curly braces
fruits = {"apple", "banana", "cherry", "apple"}
print("Fruits set:", fruits)  # Output: {'banana', 'cherry', 'apple'}

# Creating an empty set
empty_set = set()

# Using the set() function to create a set from a list
numbers = set([1, 2, 3, 4, 5, 5, 5])
print("Numbers set:", numbers)  # Output: {1, 2, 3, 4, 5}

# Adding elements to a set
fruits.add("orange")
print("After adding 'orange':", fruits)  # Output: {'banana', 'cherry', 'apple', 'orange'}

# Removing elements from a set
fruits.remove("banana")
print("After removing 'banana':", fruits)  # Output: {'cherry', 'apple', 'orange'}
```

Set Operations

```python
set_a = {1, 2, 3, 4}
set_b = {3, 4, 5, 6}

# Union: elements in either set
union_set = set_a | set_b
print("Union:", union_set)  # Output: {1, 2, 3, 4, 5, 6}

# Intersection: elements in both sets
intersection_set = set_a & set_b
print("Intersection:", intersection_set)  # Output: {3, 4}

# Difference: elements in set_a but not in set_b
difference_set = set_a - set_b
print("Difference (A - B):", difference_set)  # Output: {1, 2}

# Symmetric Difference: elements in either set, but not both
symmetric_difference_set = set_a ^ set_b
print("Symmetric Difference:", symmetric_difference_set)  # Output: {1, 2, 5, 6}
```

Set Methods

```python
fruits = {"apple", "banana", "cherry"}

# Check if an element is in the set
is_apple_in_fruits = "apple" in fruits
print("Is apple in fruits?", is_apple_in_fruits)  # Output: True

# Add multiple elements to a set
fruits.update(["orange", "grape", "apple"])
print("After update:", fruits)  # Output: {'orange', 'apple', 'grape', 'cherry', 'banana'}

# Remove an element (raises an error if the element is not present)
fruits.remove("banana")
print("After removing banana:", fruits)  # Output: {'orange', 'apple', 'grape', 'cherry'}

# Discard an element (does not raise an error if the element is not present)
fruits.discard("banana")

# Clear the set (removes all elements)
fruits.clear()
print("After clearing:", fruits)  # Output: set()
```

Practical Examples

Example 1: Removing Duplicates from a List

```python
Copy code
# Given a list with duplicate elements
numbers = [1, 2, 2, 3, 4, 4, 5]

# Convert the list to a set to remove duplicates
unique_numbers = set(numbers)
print("Unique numbers:", unique_numbers)  # Output: {1, 2, 3, 4, 5}


Example 2: Finding Common Elements in Two Lists
```
```python
Copy code
# Two lists of students in different classes
class_a = ["Alice", "Bob", "Charlie"]
class_b = ["Charlie", "David", "Alice"]

# Convert lists to sets and find the intersection
common_students = set(class_a) & set(class_b)
print("Common students:", common_students)  # Output: {'Alice', 'Charlie'}



Example 3: Checking for Subset and Superset Relationships
```
```python
Copy code
set_a = {1, 2, 3}
set_b = {1, 2, 3, 4, 5}

# Check if set_a is a subset of set_b
is_subset = set_a.issubset(set_b)
print("Is set_a a subset of set_b?", is_subset)  # Output: True

# Check if set_b is a superset of set_a
is_superset = set_b.issuperset(set_a)
print("Is set_b a superset of set_a?", is_superset)  # Output: True
```

Exercises

Exercise 1: Create and Modify a Set

```python
Copy code
# Create a set of colors
colors = {"red", "green", "blue"}

# Add a new color to the set
colors.add("yellow")

# Remove the color "green" from the set
colors.remove("green")

# Print the updated set
print("Updated colors:", colors)
Exercise 2: Find the Difference Between Two Sets
```
```python
Copy code
# Given two sets of integers
set_x = {10, 20, 30, 40}
set_y = {30, 40, 50, 60}

# Find the difference (elements in set_x but not in set_y)
difference = set_x - set_y
print("Difference (X - Y):", difference)
```