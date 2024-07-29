String notation:

```python
single_quote_string = 'Hello'
double_quote_string = "World"
triple_quote_string = '''Python programming'''
```

Creating and Using Strings

```python
name = "Alice"
greeting = 'Hello, ' + name + '!'
print(greeting)  # Output: Hello, Alice!
```

```python
multiline_string = """This is a
multiline string"""
print(multiline_string)
```

Concatenation, repetition, and indexing


```python
# Concatenation
str1 = "Hello"
str2 = "World"
result = str1 + " " + str2
print("Concatenation:", result)  # Output: Hello World
```

```python
# Repetition
result = str1 * 3
print("Repetition:", result)  # Output: HelloHelloHello
```

```python
# Indexing
first_char = str1[0]
print("First character:", first_char)  # Output: H
```

```python
# Slicing
substring = str2[1:4]
print("Slicing:", substring)  # Output: orl
```


String methods

```python
text = "  Python Programming  "

# Strip
clean_text = text.strip()
print("Strip:", clean_text)  # Output: Python Programming
```

```python
# Lowercase
lower_text = text.lower()
print("Lowercase:", lower_text)  # Output:   python programming  
```

```python
# Uppercase
upper_text = text.upper()
print("Uppercase:", upper_text)  # Output:   PYTHON PROGRAMMING  
```

```python
# Replace
replaced_text = text.replace("Python", "Java")
print("Replace:", replaced_text)  # Output:   Java Programming  
```

```python
# Split
words = text.split()
print("Split:", words)  # Output: ['Python', 'Programming']
```


Practical Examples

```python
# Formatting a String

name = "Alice"
age = 30
formatted_string = f"My name is {name} and I am {age} years old."
print("Formatted string:", formatted_string)


# Counting Words in a Sentence


sentence = "Python programming is fun and versatile."
word_count = len(sentence.split())
print("Word count:", word_count)


# Checking for Substring

text = "Hello, welcome to the world of Python!"
substring = "Python"
contains_substring = substring in text
print(f"Does the text contain '{substring}'?", contains_substring)
```

Exercises

```python

# Exercise 1: Concatenate First and Last Name

first_name = "John"
last_name = "Doe"
full_name = first_name + " " + last_name
print("Full name:", full_name)


# Exercise 2: Convert String to Uppercase and Count Length

text = "python programming"
upper_text = text.upper()
length = len(upper_text)
print("Uppercase text:", upper_text)
print("Length of text:", length)


# Exercise 3: Extract and Print Initials

name = "John Doe"
initials = name[0] + name[name.index(" ") + 1]
print("Initials:", initials)

```