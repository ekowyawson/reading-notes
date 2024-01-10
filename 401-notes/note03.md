# Class 03: FileIO & Exceptions

Understanding File Input/Output (FileIO) and Exception handling in Python is crucial for several reasons. FileIO is a fundamental part of many Python applications, as it enables interaction with files on the system, allowing for the reading, writing, and manipulation of data stored in files. This is essential in tasks ranging from simple data logging to complex data processing. Without proper handling of FileIO, a program might produce incorrect results, corrupt data, or fail to handle files that are too large or in unexpected formats. Exception handling complements this by providing a way to anticipate and manage errors that may occur during runtime, such as file not found errors, permission issues, or unexpected data formats. It ensures that the program can deal with these situations gracefully, maintaining robustness and reliability.

## [1] What is the purpose of the `with` statement when opening a file in Python, and how does it help manage resources while reading and writing files?

The with statement in Python is used for resource management and ensures that resources like file objects are properly cleaned up after their use.
When you open a file using the with statement, Python automatically takes care of closing the file once the block of code inside the `with` statement
is executed, regardless of whether an exception occurred or not. This eliminates the need to explicitly close the file and handles many of the potential
errors associated with file handling.

## [2] Explain the difference between the `read()` and `readline()` methods for file objects in Python. Provide examples of when to use each method

**`read():`** This method reads the entire content of the file into a single string. It's useful when you need to process the whole file at once or when the file size is manageable and you want to perform operations on the entire content.

Example:

```python
with open('example.txt', 'r') as file:
    content = file.read()
```

**`readline()`**: This method reads a single line from the file each time it is called. The line includes the newline character at the end. `readline()` is particularly useful for reading a file line-by-line, such as when processing or parsing a file incrementally, or when dealing with large files that shouldn’t be loaded entirely into memory.

Example:

```python
with open('example.txt', 'r') as file:
    line = file.readline()
    while line:
        print(line, end='')
        line = file.readline()
```

## [3] Briefly describe the concept of exception handling in Python. How can the `try`, `except`, and `finally` blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example

Exception handling in Python is managed using `try`, `except`, and `finally` blocks. This mechanism allows the ability to handle errors gracefully and maintain the normal flow of the code even when unexpected errors occur.

- **`try` Block**: The code that might cause an exception is placed inside the try block.

- **`except` Block**: When an exception occurs in the try block, the except block takes over and runs it's block. This is where the exception handling is defined.

- **`finally` Block**: This block is optional and is executed no matter what. It's executed whether an exception occurred or not.

Example:

```python
try:
    with open('missingFile.txt', 'r') as file:
        content = file.read()
except FileNotFoundError:
    print("File not found.")
finally:
    print("This will always be executed.")
```

## Sources

[Read & Write Files in Python](https://realpython.com/read-write-files-python/)
[Exceptions in Python](https://realpython.com/python-exceptions/)
[File Objects - Reading and Writing to Files](https://www.youtube.com/watch?v=Uh2ebFW8OYM)
[Reading and Writing Files in Python Quiz](https://realpython.com/quizzes/read-write-files-python/)

## Things I want to know more about

Nothing at this moment.
