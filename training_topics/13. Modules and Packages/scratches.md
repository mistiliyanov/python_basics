Modules and Packages

Importing Modules

```python
import math_utils
result = math_utils.add_numbers(3, 4)
print(result)
```


Importing specific functions from a module:

```python
from math_utils import add_numbers
result = add_numbers(3, 4)
print(result)
```

Renaming a module using as:

```python
import math_utils as mu
result = mu.add_numbers(3, 4)
print(result)
```

Built-in Modules:

```python
import math
print(math.sqrt(16))  # Output: 4.0

import random
print(random.randint(1, 10))  # Output: Random number between 1 and 10
```

Custom packages

```python
from utilities import math_operations, string_operations

print(math_operations.add(2, 3))  # Output: 5
print(string_operations.uppercase("hello"))  # Output: HELLO
```

Practical Example: Importing from the Standard Library and Custom Modules

```python
# my_script.py
import math
from utilities import math_operations

print("Square root of 25:", math.sqrt(25))  # Using the built-in 'math' module

# Using custom package 'utilities'
result = math_operations.add(10, 5)
print("Addition result from custom module:", result)  # Output: 15

```

Exercise: Creating and Importing a Custom Module

```python
# main.py
from greetings import say_hello

print(say_hello("Alice"))  # Output: Hello, Alice!
```

