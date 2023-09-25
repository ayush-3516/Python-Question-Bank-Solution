# Python Question Bank Solution

# Index

- [Unit - 1](#Unit-1)
    - [1. Explain Branching in context of Python.(if, else, else...if, break)](#1-explain-branching-in-context-of-pythonif-else-elseif-break)
    - [2. Discuss Control Structure in context of Python.(for, while)](#2-discuss-control-structure-in-context-of-python)
    - [3. Explain strings and operations on string type.(slicing, indexing, stride, etc..)](#3-explain-strings-and-operations-on-string-typeslicing-indexing-stride-etc)
    - [4. Explain User Defined Functions in Python](#4-explain-user-defined-functions-in-python)
    - [5. Explain Argument Passing Methods in Function. (Positional Arguments/Keyword Arguments/Default Arguments/Default Arguments/Variable Length Arguments)](#5-explain-argument-passing-methods-in-functionpositional-argumentskeyword-argumentsdefault-argumentsvariable-length-arguments)
    - [6. Discuss Scoping in terms of functions with sample code. (local/Global)](#6-discuss-scoping-in-terms-of-functions-with-sameple-codelocalglobal)
    - [7. Discuss Recursion with Example.](#7-discuss-recursion-with-example)
    - [8. What is Module? Give detailed description of it with example.](#8-what-is-module-in-python-give-detailed-description-of-it-with-example)
    - [9. Explain Files and it's access methods.](#9-explain-files-and-its-access-methods-in-python)
    - [10. Explain Function as Object.](#10-explain-function-as-object-in-python)
    - [10. How function can be passed as object? And Compare it with map()](#10-how-function-can-be-passed-as-object-and-compare-it-with-map)
    - [11. Differentiate Following Functions: (1) lambda. (2) map. (3) filter.](#11-differentiate-following-functions-ilambda-2map-3filter)
    - [11. Explain Higher Order Functions supported by Python.](#11-explain-higher-order-functions-supported-by-python)
    - [12. What is known as Mutability? Which are mutable types?](#12-what-is-known-as-mutability-which-are-mutable-types)
    - []()
    - []()
    - []()
    - []()
## Unit - 1

### **1. Explain Branching in context of Python.(if, else, else...if, break)**

Branching in Python refers to the ability to execute different sets of code based on certain conditions. This control flow feature allows you to make decisions and direct the program's execution down different paths depending on whether specific conditions are true or false.

The primary construct used for branching in Python is the `if-elif-else` statement.
Here's a breakdown of how it works:

1. `if` statement:
The `if` statement is used to execute a block of code only if a certain condition is true.

```python
if condition:
    # Code to execute if the condition is true
```

2. `elif` statement(optional):

The `elif`(short for "else if") statement allows you to specify additonal conditions to check if the first `if` condition is false.

```python
if condition1:
    # Code to execute if condition1 is true
elif condition2:
    # Code to execute if condition2 is true
```

3. `else` statement(optional):
The `else` statement is used to execute a block of code if none of the preceding conditions are true.

```python
if condition:
    # Code to execute if condition is true
else:
    # Code to execute if condition is false
```

Here's a practical example that demonstates branching:

```python
x = 10

if x > 15:
    print("x is greater than 15")
elif x > 5:
    print("x is greater than 5 but less than 15")
else:
    print("x is less than or equal to 5")
```

### **2. Discuss Control Structure in context of Python.**

In programming, control structures determine the order in which statements are executed in a program. They allow you to control the flow of execution based on conditions, loops, and function calls. Control structures are essential for creating complex programs and algorithms.

Loops allow a block of code to be executed repeatedly as long as a certain condition is met. Python supports `for` and `while` loops.

**for loop**
```python
for item in iterable:
    # Code to execute for each item in the iterable
```

**while loop**
```python
while condition:
    # Code to be executed if the condition is true
```

### **3. Explain strings and operations on string type.(slicing, indexing, stride, etc..)**

In Python, a string is a sequence of characters, and it is one of the fundamental data types used to represent text. Strings are immutable, meaning you cannot modify them in-place; you can only create new strings. Here's an explanation of strings and common operations on them:

**Strings in Python**
A string in Python can be created using single, double, or triple quotes:
```python
string1 = 'This is a string.'
string2 = "This is also a string."
string3 = """This is a multiline
string."""
```

**Accessing Characters in a String(Indexing)**
Every character in a string is associated with an index (position) starting from 0 for the first character. You can access individual characters by their index using square brackets [].
```python
my_string = "Hello, World!"

# Accessing individual characters
print(my_string[0])  # Output: 'H'
print(my_string[7])  # Output: 'W'
```

**Slicing**
Slicing allows you to extract a portion(substring) of a string by specifying a range of indices.
```python
my_string = "Hello, World!"

# Slicing syntax: string[start:end:step]
print(my_string[0:5])   # Output: 'Hello'
print(my_string[7:])    # Output: 'World!'
print(my_string[:5])    # Output: 'Hello'
print(my_string[::2])   # Output: 'Hlo ol!'
```

**Stride**
Stride(also known as a step) is the number of characters to skip while slicing.
```python
my_string = "Hello, World!"

print(my_string[::2])  # Output: 'HloWrd'    
```

**String Length**
You can find the length of a string(the number of characters in the string) using the `len()` function.
```python
my_string = "Hello, World!"
print(len(my_string))  # Output: 13
```

**Concatenation**
Strings can be concatenated using the `+` operator.
```python
string1 = "Hello, "
string2 = "World!"
concatenated_string = string1 + string2
print(concatenated_string)  # Output: 'Hello, World!'
```

### **4. Explain User-Defined Functions in Python.**

A user-defined function is a block of reusable code that performs a specific task or a set of tasks. Functions help organize and modularize code, making it easier to manage, debug, and reuse. Defining your own functions allows you to create custom operations and functionalities tailored to your specific needs. Here's a detailed explanation of how to define and use user-defined functions in Python:

**Defining a Function**

To define a function in Python, you use the `def` keyword followed by the function name, parenthesis for parameters, a colon, and then the function body, indented appropriately.
```python
def function_name(parameter1, parameter2, ...):
    # Function body
    # Code to perform a specific task
    return result  # optional return statement
```

### **5. Explain Argument Passing methods in function.(Positional Arguments/Keyword Arguments/Default Arguments/Variable Length Arguments)**

In Python, when you call a function, you can pass arguments to the function in several ways: positional arguments, keyword arguments, default arguments, and variable-length arguments. These methods give you flexibility in how you provide input to a function. Let's discuss each method in detail:

**1. Positional Arguments:**

Positional arguments are the most common way of passing arguments to a function. The order of the arguments matters, and the values are assigned to the parameters based on their positions.

Example:

```python
def greet(name, greeting):
    return f"{greeting}, {name}!"

# Calling the function using positional arguments
message = greet("Alice", "Hello")
print(message)  # Output: Hello, Alice!
```

**2. Keyword Arguments:**

Keyword arguments are passed to a function using the format `parameter_name=value`. This method allows you to pass arguments in any order, making the function call more readable and self-explanatory.

Example:

```python
# Calling the function using keyword arguments
message = greet(greeting="Hi", name="Bob")
print(message)  # Output: Hi, Bob!
```

**3. Default Arguments:**

Default arguments have predefined values set in the function definition. If a value is not provided for a parameter during the function call, the default value is used.

Example:

```python
def greet(name, greeting="Hello"):
    return f"{greeting}, {name}!"

# Calling the function without specifying greeting (uses default)
message = greet("Alice")
print(message)  # Output: Hello, Alice!

# Calling the function with a custom greeting
message = greet("Alice", "Hi")
print(message)  # Output: Hi, Alice!
```

**4. Variable Length Arguments:**

Python allows functions to accept a variable number of arguments. There are two types of variable-length arguments: arbitrary positional arguments and arbitrary keyword arguments.

a. Arbitrary Positional Arguments:
You can define a function that accepts an arbitrary number of positional arguments using an asterisk (*). These arguments are received as a tuple.

Example:

```python
def sum_all(*args):
    total = 0
    for num in args:
        total += num
    return total

# Calling the function with variable number of arguments
result = sum_all(1, 2, 3, 4)
print(result)  # Output: 10
```

b. Arbitrary Keyword Arguments:

You can define a function that accepts an arbitrary number of keyword arguments using double asterisks(`**`). These arguments are recieved as a dictionary.

```python
def display_info(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

# Calling the function with variable number of keyword arguments
display_info(name="Alice", age=30, city="New York")
```

### **6. Discuss Scoping in terms of functions with sameple code.(local/Global)**

In Python, scoping refers to the accessibility of variables in different parts of the code. Variables in Python can have either local scope or global scope, depending on where they are defined. Let's discuss local and global scoping in the context of functions and provide sample code for better understanding.

**Local Scope**
Variable defined within a function have a local scope. This means they are accessible only within that function and cannot be accessed outside of it.

```python
def my_function():
    x = 10  # Local variable
    print(x)

my_function()
print(x)  # This will raise a NameError because x is not defined in this scope
```

**Global Scope**
Variables defined outside of any function have a global scope. They can be accessed and modified anywhere in the code.

```python
y = 20  # Global variable

def another_function():
    print(y)

another_function()
print(y)  # Output: 20
```

### **7. Discuss Recursion with example.**

Recursion is a programming concept where a function calls itself in order to solve a problem. This technique allows solving complex problems by breaking them down into simpler, similar subproblems. In the context of programming, recursion often involves a base case to stop the recursion and prevent an infinite loop.

Here's a detailed explanation of recursion with a simple example in Python: the factorial calculation using recursion.

**Factorial Calculation Using Recursion.**

The factorial of a non-negative integer `n` (denoted as `n!`) is the product of all positive integers from 1 to `n`. Mathematically, `n! = n * (n-1) * (n-2) * ... * 1`.

Let's create a recursive function to calculate the factorial of a given non-negative integer:

```python
def factorial(n):
    # Base case: factorial of 0 or 1 is 1
    if n == 0 or n == 1:
        return 1
    else:
        # Recursive call to calculate factorial
        return n * factorial(n - 1)

# Calculate factorial of 5
result = factorial(5)
print("Factorial of 5 is:", result)  # Output: Factorial of 5 is: 120
```

### **8. What is Module in Python? Give detailed description of it with example.**

In Python, a module is a file that contains Python definitions, statements, and functions. Modules allow you to organize code into separate files, making it easier to manage, reuse, and distribute functionality across different parts of a program or different programs. A module can contain variables, functions, classes, and other objects.

**Creating a Module**
To create a module, you simply create a Python file with a `.py` extension. This file will serve as your module, containing the functions, variables, or other elements you want to encapsulate.

Example Module - `my_module.py`:

```python
# my_module.py

def greet(name):
    return f"Hello, {name}!"

def add(a, b):
    return a + b

# This variable is also part of the module
PI = 3.14159
```

In this example, `my_module.py` is a module containing `greet()`, `add()`, and `PI`. These can be imported into other Python scripts for use.

**Importing a Module**
To use the functions and variables from a module in another Python script, you need to import the module using the `import` statement.

Example - Using the Module:

```python
import my_module

# Using functions from the module
print(my_module.greet("Alice"))  # Output: Hello, Alice!
print(my_module.add(3, 5))        # Output: 8

# Using variables from the module
print(my_module.PI)               # Output: 3.14159
```

You can also import specific functions or variables from a module using the `from` keyword.

```python
from my_module import greet, PI

print(greet("Bob"))  # Output: Hello, Bob!
print(PI)             # Output: 3.14159
```

### **9. Explain Files and it's access methods in Python.**

In Python, working with files involves reading from and writing to external files on the file system. Files are essential for data storage, data processing, and communication between programs and the external environment. Python provides various methods and functions to work with files, allowing you to read, write, and manage file data effectively.

**File Basics**

- Opening a File

To open a file, you use the `open()` function, specifying the file path and mode (e.g., read, write, append, etc.).

```python
file = open('example.txt', 'r')  # Opens for reading ('r' is the default mode)
```

Modes for open()

'r': Read (default)

'w': Write (overwrites existing content)

'a': Append (appends to existing content)

'b': Binary mode

't': Text mode (default)

'x': Exclusive creation, if the file already exists, the operation will fail

- Closing a File

It's important to close a file after you're done with it to free up system resources.
```python
file.close()
```

**File Reading**

Reading Entire Contents:
```python
file = open('example.txt', 'r')
content = file.read()  # Reads the entire content of the file as a string
file.close()
print(content)
```

Reading Lines:
```python
file = open('example.txt', 'r')
lines = file.readlines()  # Reads the lines of the file and returns a list
file.close()
for line in lines:
    print(line.strip())  # Strips newline characters and prints each line
```

**File Writing**

Writing a File:
```python
file = open('output.txt', 'w')  # Opens for writing
file.write('This is some content.\n')
file.close()
```

Appending to a File:
```python
file = open('output.txt', 'a')  # Opens for appending
file.write('This is additional content.\n')
file.close()
```

**File Iteration**

You can interate through lines in a file directly using a `for` loop.
```python
file = open('example.txt', 'r')
for line in file:
    print(line.strip())
file.close()
```

**Using `with` statement**
The `with` statement automatically closes the file after exiting the block, even if an exception occurs.
```python
with open('example.txt', 'r') as file:
    content = file.read()
    print(content)
```

**File Methods and Attributes**

`read(size)`: Reads and returns size number of bytes from the file.

`readline()`: Reads a line from the file.

`readlines()`: Reads all lines of the file and returns them as a list.

`write(string)`: Writes the string to the file.

`tell()`: Returns the current file pointer position.

`seek(offset, from)`: Moves the file pointer to a specified position (from the beginning, end, or current position).

**Binary Files**

To work with binary files, you can use the 'b' mode and read/write binary data.

```python
with open('binary_file.bin', 'wb') as file:
    file.write(b'Binary data')
```

### **10. Explain Function as Object in Python.**

OR

### **10. How function can be passed as Object? And compare it with map().**

In Python, functions are first-class citizens, which means they can be treated like any other object. This includes passing functions as arguments to other functions, returning functions from functions, and storing them in data structures. This powerful feature allows for functional programming paradigms and enhances the flexibility and expressiveness of the language.

**Passing a Function as an Object**
Here's an example demonstrating how to pass a function as an object (argument) to another function:

```python
def greet(name):
    return f"Hello, {name}!"

def process_greeting(greeter, name):
    return greeter(name)

# Pass the greet function as an argument to process_greeting
message = process_greeting(greet, "Alice")
print(message)  # Output: Hello, Alice!
```

**Comparison with `map()`**

`map()` is a built-in Python function that allows you to apply a specified function to every item in an iterable (e.g., a list) and return an iterator that yields the results.

Here's an example of using `map()` to apply a function to a list of names:

```python
def greet(name):
    return f"Hello, {name}!"

names = ["Alice", "Bob", "Charlie"]

# Using map to apply the greet function to each name in the list
greetings = map(greet, names)

# Convert the map iterator to a list to see the results
greetings_list = list(greetings)
print(greetings_list)
# Output: ['Hello, Alice!', 'Hello, Bob!', 'Hello, Charlie!']
```

### **11. Differentiate following functions: (i)lambda. (2)map. (3)filter.**

In Python, `lambda`, `map`, and `filter` are functional programming constructs used for data manipulation and transformation. Each serves a different purpose and has distinct characteristics:

**Lambda Functions**
- Purpose: Lambda functions, also known as anonymous functions, are used to create small, one-time-use functions without a formal function definition.

- Syntax: `lambda arguments: expression`

- Example:
```python
square = lambda x: x**2
print(square(5))  # Output: 25
```

- Characteristics:
    - Concise and ofter used in simple operations.
    - Cannot contain multiple expressions or statements.
    - Typically used for short, one-line operations.

**Map**

- Purpose: The `map()` function is used to apply a given function to each element in an iterable(e.g., a list) and returns an iterator that yields the transformed elements.

- Syntax: `map(function, iterable(s))`

- Example:
```python
numbers = [1, 2, 3, 4]
double_numbers = map(lambda x: x * 2, numbers)
print(list(double_numbers))  # Output: [2, 4, 6, 8]
```

- Characteristics:
    - Applies a function to each element in the iterable.
    - Returns an iterator, so it's memory efficient for large datasets.
    - Tyically used for element-wise transformations.

**Filter**

- Purpose: The `filter()` function is used to construct an iterator from elements of an iterable for which a function returns true.

- Syntax: `filter(function, iterable)`

- Example:
```python
numbers = [1, 2, 3, 4, 5, 6]
even_numbers = filter(lambda x: x % 2 == 0, numbers)
print(list(even_numbers))  # Output: [2, 4, 6]
```

- Characteristics:
    - Filters elements based on the provided function(which should return a boolean).
    - Returns an iterator, so it's memory  efficient for large datasets.
    - Typically used for filtering based on a condition.

-------- OR ---------

### **11. Explain Higher Order Functions supported by Python.**

In Python, a higher-order function is a function that meets at least one of the following criteria:

1. Takes a Function as an Argument:

The higher-order function takes one or more functions as arguments.

2. Returns a Function:

The higher-order function returns a function as its result.

Higher-order functions are a fundamental concept in functional programming and provide a powerful way to abstract and compose functionality.

Example 1: Function as an Argument

```python
def apply_operation(operation, x):
    return operation(x)

def double(x):
    return 2 * x

def square(x):
    return x ** 2

result1 = apply_operation(double, 3)  # Passing 'double' function
result2 = apply_operation(square, 4)  # Passing 'square' function

print(result1)  # Output: 6
print(result2)  # Output: 16
```

Example 2: Function as a Result

```python
def make_adder(n):
    def adder(x):
        return x + n
    return adder

add_5 = make_adder(5)
add_10 = make_adder(10)

result1 = add_5(3)  # Output: 8
result2 = add_10(3)  # Output: 13

print(result1)
print(result2)
```

### **12. What is known as Mutability? Which are mutable types?**

In programming, mutability refers to the ability of an object or data structure to be changed or modified after its creation. If a data type or object is mutable, it means that its state can be altered, elements can be added or removed, and its contents can be modified in-place without creating a new instance.

Conversely, immutability refers to the characteristic of not being able to be changed after creation. Immutable objects cannot have their state altered once they are created.

**Mutable Types in Python**

In Python, some data types are mutable, meaning they can be modified after creation, while others are immutable and cannot be changed. Here are some common examples of mutable and immutable types in Python:

Mutable Types:

Lists (`list`):

Lists are ordered collections of items, and their elements can be modified, added, or removed after creation.
```python
my_list = [1, 2, 3]
my_list[0] = 5  # Modifying an element
my_list.append(4)  # Adding an element
```


