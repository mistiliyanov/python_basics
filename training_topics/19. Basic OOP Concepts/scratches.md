Basic OOP Concepts (Classes and Objects)


Understanding Classes and Objects

Instantiating classes

```python

class Dog:
    pass

```


Creating a Basic Class

```python
class Dog:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def bark(self):
        print(f"{self.name} says Woof!")

```

Creating an Object (Instance)

```python

my_dog = Dog("Buddy", 5)
print(my_dog.name)  # Output: Buddy
print(my_dog.age)   # Output: 5
my_dog.bark()       # Output: Buddy says Woof!

```
Attributes in OOP

```python

another_dog = Dog("Bella", 3)
print(another_dog.name)  # Output: Bella

```

Methods in OOP


```python
class Dog:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def bark(self):
        print(f"{self.name} says Woof!")

    def birthday(self):
        self.age += 1
        print(f"Happy Birthday {self.name}! You are now {self.age} years old.")

```

Practical Example – Creating a Simple Class

```python

class Car:
    def __init__(self, make, model, year):
        self.make = make
        self.model = model
        self.year = year
        self.odometer = 0

    def drive(self, miles):
        self.odometer += miles
        print(f"You've driven {miles} miles. Odometer now reads {self.odometer} miles.")

    def get_info(self):
        return f"{self.year} {self.make} {self.model}"


```
Usage:

```python

my_car = Car("Toyota", "Corolla", 2020)
print(my_car.get_info())  # Output: 2020 Toyota Corolla
my_car.drive(100)         # Output: You've driven 100 miles. Odometer now reads 100 miles.


```

Exercise: Creating Your Own Class

```python

class Book:
    def __init__(self, title, author, pages):
        self.title = title
        self.author = author
        self.pages = pages

    def summary(self):
        print(f"{self.title} by {self.author}, {self.pages} pages long.")


```
Usage: 

```python

my_book = Book("The Count of Monte Cristo", "Alexandre Dumas", 1150)
my_book.summary()

```
