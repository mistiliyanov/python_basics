What are Loops?

```python
# Repeat a task multiple times using a loop
for item in sequence:
    # Perform an action
```

for Loops

```python
# Iterating over a list
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
    
# Iterating over a range of numbers
for i in range(1, 6):
    print(i)
```

while Loops

```python
# Example of a while loop
count = 1
while count <= 5:
    print(count)
    count += 1  # Increment the counter
```


Loop Control: break, continue, and else


```python
for number in range(1, 10):
    if number == 5:
        break  # Exit the loop
    print(number)

```


```python
for number in range(1, 10):
    if number == 5:
        continue  # Skip the rest of the code in this iteration
    print(number)

```


```python
for number in range(1, 5):
    print(number)
else:
    print("Loop completed successfully!")

```

Practical Examples


```python
# Example 1: Summing Numbers with a for Loop

numbers = [1, 2, 3, 4, 5]
total = 0

for num in numbers:
    total += num

print("Total sum:", total)  # Output: 15

```


```python
# Simple Password Checker with a while Loop

correct_password = "python123"
attempt = ""

while attempt != correct_password:
    attempt = input("Enter password: ")

print("Access granted.")

```

```python
# Nested for Loop for a Multiplication Table

for i in range(1, 4):
    for j in range(1, 4):
        print(f"{i} x {j} = {i * j}")

```

Exercises


Exercise 1: Loop Through a List

```python
# Write a loop that prints each item in the list.
animals = ["dog", "cat", "elephant"]

# Your code here
for animal in animals:
    print(animal)
```

Exercise 2: Find the Factorial of a Number
```python
# Write a program that uses a loop to calculate the factorial of a given number.
number = 5
factorial = 1

# Your code here
for i in range(1, number + 1):
    factorial *= i

print(f"The factorial of {number} is {factorial}")
```

Exercise 3: Guess the Number Game

```python
# Create a guessing game where the user must guess a number between 1 and 10.
import random

secret_number = random.randint(1, 10)
guess = 0

while guess != secret_number:
    guess = int(input("Guess the number (1-10): "))

print("Congratulations, you guessed it!")
```