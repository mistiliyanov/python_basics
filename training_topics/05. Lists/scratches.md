Lists
List types

```python
numbers = [1, 2, 3, 4, 5]
fruits = ["apple", "banana", "cherry"]
mixed = [1, "hello", 3.14, True]
```

Creating and Using Lists

```python
# Creating lists
empty_list = []
numbers = [1, 2, 3, 4, 5]
fruits = ["apple", "banana", "cherry"]

# Accessing elements by index
first_number = numbers[0]
print("First number:", first_number)  # Output: 1

# Slicing a list
first_two_numbers = numbers[:2]
print("First two numbers:", first_two_numbers)  # Output: [1, 2]

# Looping through a list
for fruit in fruits:
    print("Fruit:", fruit)
```

List Operations

```python
# Concatenation
list1 = [1, 2, 3]
list2 = [4, 5, 6]
combined_list = list1 + list2
print("Concatenation:", combined_list)  # Output: [1, 2, 3, 4, 5, 6]

# Repetition
repeated_list = list1 * 2
print("Repetition:", repeated_list)  # Output: [1, 2, 3, 1, 2, 3]

# Membership testing
is_in_list = 2 in list1
print("Is 2 in list1?", is_in_list)  # Output: True
```

List Methods

```python
numbers = [1, 2, 3, 4, 5]

# Append an item to the list
numbers.append(6)
print("Append:", numbers)  # Output: [1, 2, 3, 4, 5, 6]

# Insert an item at a specific position
numbers.insert(2, 2.5)
print("Insert:", numbers)  # Output: [1, 2, 2.5, 3, 4, 5, 6]

# Remove an item from the list
numbers.remove(2.5)
print("Remove:", numbers)  # Output: [1, 2, 3, 4, 5, 6]

# Pop an item from the list
last_number = numbers.pop()
print("Pop:", last_number)  # Output: 6
print("List after pop:", numbers)  # Output: [1, 2, 3, 4, 5]

# Find the index of an item
index_of_three = numbers.index(3)
print("Index of 3:", index_of_three)  # Output: 2

# Sort the list
numbers.sort()
print("Sorted list:", numbers)  # Output: [1, 2, 3, 4, 5]

# Reverse the list
numbers.reverse()
print("Reversed list:", numbers)  # Output: [5, 4, 3, 2, 1]
```

Practical Examples

```python
# Example 1: Calculating the Sum of a List of Numbers

numbers = [10, 20, 30, 40, 50]
total = sum(numbers)
print("Sum of numbers:", total)


# Example 2: Finding the Maximum and Minimum Values in a List

values = [10, 3, 25, 7, 18]
max_value = max(values)
min_value = min(values)
print("Max value:", max_value)  # Output: 25
print("Min value:", min_value)  # Output: 3


# Example 3: List Comprehensions

# Create a list of squares of numbers from 1 to 5
squares = [x**2 for x in range(1, 6)]
print("Squares:", squares)  # Output: [1, 4, 9, 16, 25]
```

Exercises


```python
# Exercise 1: Create and Modify a List

# Create a list of your favorite fruits
favorite_fruits = ["apple", "banana", "mango"]

# Add a new fruit to the list
favorite_fruits.append("orange")

# Remove a fruit from the list
favorite_fruits.remove("banana")

# Print the updated list
print("Updated list of favorite fruits:", favorite_fruits)


# Exercise 2: List Operations and Methods

# Create a list of numbers from 1 to 10
numbers = list(range(1, 11))

# Find and print the sum of the numbers
total_sum = sum(numbers)
print("Sum:", total_sum)

# Find and print the maximum number in the list
max_num = max(numbers)
print("Max number:", max_num)

# Reverse the list and print it
numbers.reverse()
print("Reversed list:", numbers)
```

