### Arithmetic Operations

```python
a = 10
b = 3

print("Addition:", a + b)        # 13
print("Subtraction:", a - b)     # 7
print("Multiplication:", a * b)  # 30
print("Division:", a / b)        # 3.3333...
print("Modulus:", a % b)         # 1
print("Exponentiation:", a ** b) # 1000
print("Floor Division:", a // b) # 3
```

```python
# find side A in a right angled triangle "A^2 + B^2 = C^2"
def find_a(b, c):
    a = (c ** 2 - b ** 2) ** 0.5
    return a

find_a(4, 5)
```


### Comparison Operations

```python
x = 5
y = 8

print("Equal:", x == y)              # False
print("Not equal:", x != y)          # True
print("Greater than:", x > y)        # False
print("Less than:", x < y)           # True
print("Greater or equal:", x >= y)   # False
print("Less or equal:", x <= y)      # True
```

### Logical Operations

```python
a = True
b = False

print("a and b:", a and b)  # False
print("a or b:", a or b)    # True
print("not a:", not a)      # False
```

### Assignment Operations

```python
x = 10

x += 5  # x = x + 5
print("x += 5:", x)  # 15

x -= 3  # x = x - 3
print("x -= 3:", x)  # 12

x *= 2  # x = x * 2
print("x *= 2:", x)  # 24

x /= 4  # x = x / 4
print("x /= 4:", x)  # 6.0

x %= 2  # x = x % 2
print("x %= 2:", x)  # 0.0

x **= 3  # x = x ** 3
print("x **= 3:", x)  # 0.0

x //= 1  # x = x // 1
print("x //= 1:", x)  # 0.0
```

### Practical Examples

#### Calculating the Average of Three Numbers
```python
num1 = 85
num2 = 90
num3 = 78

average = (num1 + num2 + num3) / 3
print("Average:", average)
```

#### Checking Eligibility for a Discount
```python
age = 65
is_member = True

eligible_for_discount = (age >= 60) or is_member
print("Eligible for discount:", eligible_for_discount)
```

#### Updating Inventory
```python
inventory = 100

# A sale of 20 items
inventory -= 20
print("Updated inventory after sale:", inventory)

# A restock of 50 items
inventory += 50
print("Updated inventory after restock:", inventory)
```

### Exercises

#### Basic Arithmetic

```python
a = 15
b = 4

# Perform addition, subtraction, multiplication, and division
sum_ab = a + b
diff_ab = a - b
prod_ab = a * b
quot_ab = a / b

# Print the results
print("Sum:", sum_ab)
print("Difference:", diff_ab)
print("Product:", prod_ab)
print("Quotient:", quot_ab)
```

#### Logical Comparisons
```python
x = 10
y = 20
z = 15

# Check if x is less than y and z is greater than y
result = (x < y) and (z > y)
print("Result of (x < y) and (z > y):", result)

# Check if x is equal to 10 or y is less than 15
result = (x == 10) or (y < 15)
print("Result of (x == 10) or (y < 15):", result)
```

