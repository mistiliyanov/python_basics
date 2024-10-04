File Handling

Opening and Closing Files


```python
file = open("filename.txt", "mode")
file.close()

```
"r": Read (default)
"w": Write (overwrites)
"a": Append (adds data to the end)
"r+": Read and write

```python
file = open("example.txt", "r")
# Perform file operations
file.close()
```

Using the with Statement

```python
with open("example.txt", "r") as file:
    content = file.read()
# No need to explicitly close the file

```

Reading from Files


```python
with open("example.txt", "r") as file:
    content = file.read()  # Reads the entire file
    print(content)

```

Writing to Files


```python

with open("output.txt", "w") as file:
    file.write("Hello, World!\n")
```

Practical Example: Read from and Write to a File


```python
# Reading from input.txt and writing to output.txt
with open("input.txt", "r") as infile:
    content = infile.read()

with open("output.txt", "w") as outfile:
    outfile.write(content.upper())  # Writes content in uppercase

```

Exercise: Read and Write to a File

Reverse lines:
```python
with open("data.txt", "r") as file:
    for line in file:
        print(line[::-1])  # Reverse each line and print

```

