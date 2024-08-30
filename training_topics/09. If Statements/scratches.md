What are If Statements?

```python
# Simple if statement
x = 10
if x > 5:
    print("x is greater than 5")

```

Basic Syntax and Usage

age = 18

```python
# Check if age is 18 or older
if age >= 18:
    print("You are an adult.")
```

'else' and 'elif' Clauses

```python
temperature = 30

if temperature > 30:
    print("It's hot outside.")
elif temperature > 20:
    print("It's warm outside.")
else:
    print("It's cold outside.")
```


Nested If Statements

```python
score = 85

if score >= 60:
    print("You passed!")
    if score >= 90:
        print("You got an A!")
    elif score >= 80:
        print("You got a B!")
else:
    print("You failed.")
```

Practical Examples

Example 1: Checking for Even or Odd Number

```python
number = 7

if number % 2 == 0:
    print("The number is even.")
else:
    print("The number is odd.")
```

Example 2: Validating User Input

```python
password = input("Enter your password: ")

if len(password) < 8:
    print("Password is too short.")
else:
    print("Password length is acceptable.")
```

Example 3: Determining the Largest of Three Numbers

```python
a = 10
b = 20
c = 15

if a > b and a > c:
    print("a is the largest.")
elif b > c:
    print("b is the largest.")
else:
    print("c is the largest.")
```

Exercises

Exercise 1: Basic If Statement

```python
# Write a program that checks if a number is positive, negative, or zero.
number = 5

# Your code here
if number > 0:
    print("The number is positive.")
elif number < 0:
    print("The number is negative.")
else:
    print("The number is zero.")
```

Exercise 2: Temperature Check

```python
# Write a program that checks the temperature and prints appropriate clothing advice.
temperature = 15

# Your code here
if temperature >= 25:
    print("Wear shorts and a t-shirt.")
elif temperature >= 15:
    print("Wear a light jacket.")
else:
    print("Wear a warm coat.")
```

Exercise 3: Age Group Classification

```python
# Write a program that categorizes a person's age into different age groups.
age = 45

# Your code here
if age < 13:
    print("You are a child.")
elif age < 20:
    print("You are a teenager.")
elif age < 65:
    print("You are an adult.")
else:
    print("You are a senior.")
```