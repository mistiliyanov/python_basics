What are Dictionaries?

```python
# Creating a dictionary
student = {"name": "Alice", "age": 25, "grade": "A"}

# Another example
phone_book = {"John": "555-1234", "Jane": "555-5678", "Alice": "555-8765"}
```

Creating and Using Dictionaries

```python
# Creating a dictionary
student = {"name": "Alice", "age": 25, "grade": "A"}

# Accessing values by key
student_name = student["name"]
print("Student's name:", student_name)  # Output: Alice

# Adding a new key-value pair
student["major"] = "Computer Science"
print("Updated student info:", student)

# Updating an existing value
student["grade"] = "A+"
print("Updated grade:", student["grade"])

# Removing a key-value pair
del student["age"]
print("After removing age:", student)
```


Dictionary Operations

```python
student = {"name": "Alice", "age": 25, "grade": "A"}

# Check if a key exists
has_age = "age" in student
print("Does 'age' exist?", has_age)  # Output: True

# Get the number of key-value pairs
num_items = len(student)
print("Number of items in the dictionary:", num_items)  # Output: 3

# Merge two dictionaries
additional_info = {"graduation_year": 2024, "GPA": 3.9}
student.update(additional_info)
print("Merged dictionary:", student)
```

Dictionary Methods

```python
student = {"name": "Alice", "age": 25, "grade": "A"}

# Get a value with a default if the key doesn't exist
major = student.get("major", "Undeclared")
print("Major:", major)  # Output: Undeclared

# Remove and return a value by key
grade = student.pop("grade")
print("Popped grade:", grade)  # Output: A
print("After pop:", student)

# Get all keys, values, or key-value pairs
keys = student.keys()
values = student.values()
items = student.items()
print("Keys:", keys)
print("Values:", values)
print("Items:", items)
```

Practical Examples

Example 1: Counting the Frequency of Words

```python
text = "hello world hello"
word_count = {}

for word in text.split():
    if word in word_count:
        word_count[word] += 1
    else:
        word_count[word] = 1

print("Word count:", word_count)  # Output: {'hello': 2, 'world': 1}
```

Example 2: Storing and Accessing Data

```python
# A dictionary of students and their grades
grades = {"Alice": "A", "Bob": "B", "Charlie": "C"}

# Accessing a student's grade
alice_grade = grades["Alice"]
print("Alice's grade:", alice_grade)  # Output: A
```

Example 3: Dictionary Comprehension

```python
# Create a dictionary with squares of numbers from 1 to 5
squares = {x: x**2 for x in range(1, 6)}
print("Squares:", squares)  # Output: {1: 1, 2: 4, 3: 9, 4: 16, 5: 25}
```

Exercises

Exercise 1: Create and Modify a Dictionary

```python
# Create a dictionary to store information about a book
book_info = {
    "title": "1984",
    "author": "George Orwell",
    "year_published": 1949
}

# Add the genre of the book
book_info["genre"] = "Dystopian"

# Update the year published
book_info["year_published"] = 1950

# Print the updated dictionary
print("Updated book info:", book_info)
```

Exercise 2: Counting Items

```python
# Given a list of fruits
fruits = ["apple", "banana", "orange", "apple", "orange", "banana", "apple"]

# Create a dictionary to count the frequency of each fruit
fruit_count = {}

for fruit in fruits:
    if fruit in fruit_count:
        fruit_count[fruit] += 1
    else:
        fruit_count[fruit] = 1

print("Fruit count:", fruit_count)
```


