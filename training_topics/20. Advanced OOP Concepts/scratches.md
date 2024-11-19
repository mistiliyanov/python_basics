Advanced OOP Concepts 
(Inheritance, Polymorphism, Encapsulation)


Basic OOP Concepts recap

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


another_dog = Dog("Bella", 3)
print(another_dog.name)  # Output: Bella
```

Inheritance:


```python

class Animal:
    def __init__(self, name):
        self.name = name

    def make_sound(self):
        return "Some sound"

class Dog(Animal):
    def make_sound(self):
        return "Woof!"

my_dog = Dog("Buddy")
print(my_dog.make_sound())  # Output: Woof!


```

Polymorphism:

```python

class Cat(Animal):
    def make_sound(self):
        return "Meow!"

my_cat = Cat("Whiskers")
animals = [my_dog, my_cat]

for animal in animals:
    print(animal.make_sound())  # Output: Woof! and Meow!


```

Encapsulation:

```python

class BankAccount:
    def __init__(self, balance):
        self.__balance = balance  # Private attribute

    def deposit(self, amount):
        if amount > 0:
            self.__balance += amount
            print(f"Deposited: ${amount}")
        else:
            print("Invalid deposit amount")

    def get_balance(self):
        return self.__balance

account = BankAccount(1000)
account.deposit(500)
print(account.get_balance())  # Output: 1500


```

Practical Example – Implementing Advanced OOP Concepts


```python

class Employee:
    def __init__(self, name, salary):
        self.name = name
        self._salary = salary

    def work(self):
        pass

class Developer(Employee):
    def work(self):
        print(f"{self.name} is coding.")

class Manager(Employee):
    def work(self):
        print(f"{self.name} is managing a team.")


```
call methods:

```python

dev = Developer("Alice", 70000)
mgr = Manager("Bob", 90000)

employees = [dev, mgr]
for emp in employees:
    emp.work()  # Output: Alice is coding, Bob is managing a team


```

Exercise: Implementing Encapsulation


```python

class Car:
    def __init__(self, fuel_level=0):
        self.__fuel_level = fuel_level
        self.__mileage = 0

    def drive(self, distance):
        if self.__fuel_level > distance / 10:
            self.__mileage += distance
            self.__fuel_level -= distance / 10
            print(f"Drove {distance} miles. Remaining fuel: {self.__fuel_level} liters.")
        else:
            print("Not enough fuel!")

    def refuel(self, liters):
        self.__fuel_level += liters
        print(f"Refueled with {liters} liters.")


```
