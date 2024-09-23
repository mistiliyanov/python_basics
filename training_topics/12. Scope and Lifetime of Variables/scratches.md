Scope and Lifetime of Variables

What is scope?
```python
def example_function():
    x = 10  # Variable 'x' is only accessible inside this function

example_function()
print(x)  # Error: 'x' is not defined outside the function
```

Global vs. Local Variables


```python
x = 5  # Global variable

def my_function():
    print(x)  # Accessing the global variable 'x'

my_function()  # Output: 5

```

```python
def my_function():
    y = 10  # Local variable
    print(y)

my_function()  # Output: 10
print(y)  # Error: 'y' is not defined outside the function

```

Modifying Global Variables

```python
x = 10  # Global variable

def modify_global():
    global x  # Declare that we want to modify the global 'x'
    x = 20

modify_global()
print(x)  # Output: 20
```

Enclosing (Nonlocal) Scope

```python
def outer_function():
    x = "outer"
    
    def inner_function():
        nonlocal x  # Modify the variable from the enclosing (outer) function
        x = "inner"
        
    inner_function()
    print(x)  # Output: inner

outer_function()

```

Lifetime of Variables


```python
def my_function():
    x = 10  # Local variable
    print(x)

my_function()  # Output: 10
print(x)  # Error: 'x' is not defined (the local variable 'x' no longer exists)

```

Practical Examples

```python
# Counting Function Calls with Global Variables

counter = 0  # Global variable

def increment_counter():
    global counter  # Modify global variable
    counter += 1

increment_counter()
increment_counter()
print(counter)  # Output: 2

```

```python
# Using Local and Global Variables Together

x = "global"

def print_variables():
    y = "local"  # Local variable
    print("Inside function:", x)  # Accessing global variable
    print("Inside function:", y)  # Accessing local variable

print_variables()
print("Outside function:", x)  # Output: global
# print("Outside function:", y)  # Error: 'y' is not defined

```

Exercises

Global and Local Variables

```python
# Define a global variable and a local variable inside a function. Modify the global variable inside the function using the 'global' keyword.

x = 5  # Global variable

def modify_variable():
    global x
    x = 10  # Modify global variable

modify_variable()
print(x)  # Output: 10

```

Nested Functions with nonlocal

```python
# Create a nested function and modify the enclosing variable using the 'nonlocal' keyword.

def outer():
    a = 5
    
    def inner():
        nonlocal a
        a = 10
    
    inner()
    print(a)  # Output: 10

outer()

```