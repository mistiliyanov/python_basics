Error Handling

Common Errors

```python
# Example of ValueError
int("abc")  # Can't convert a string to an integer


```
```python
try:
    number = int(input("Enter a number: "))
except ValueError:
    print("That was not a valid number!")
else:
    print("You entered:", number)
finally:
    print("Execution complete.")

```

Catching Specific Exceptions

```python
try:
    x = 10 / 0
except ZeroDivisionError:
    print("You can't divide by zero!")
except ValueError:
    print("Value error occurred!")
except Exception as e:
    print(f"An unexpected error occurred: {e}")

```

Raising Exceptions

```python
def check_age(age):
    if age < 0:
        raise ValueError("Age cannot be negative.")
    return age

try:
    age = check_age(-5)
except ValueError as e:
    print(f"Error: {e}")
```

The finally Block

```python
try:
    file = open("example.txt", "r")
    # File operations
except FileNotFoundError:
    print("File not found.")
finally:
    file.close()  # This will always run, ensuring the file is closed
```


Practical Example: Handling File Operations

```python
try:
    with open("nonexistent_file.txt", "r") as file:
        content = file.read()
except FileNotFoundError:
    print("The file you are trying to open does not exist.")
except Exception as e:
    print(f"An unexpected error occurred: {e}")

```

Exercise: Catching and Raising Exceptions

```python
def square_number(num):
    if num < 0:
        raise ValueError("The number cannot be negative.")
    return num ** 2

try:
    number = int(input("Enter a number: "))
    result = square_number(number)
    print("The square of the number is:", result)
except ValueError as e:
    print(f"Error: {e}")
```

