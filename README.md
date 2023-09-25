# Python Question Bank Solution

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

### **6. Discuss Recursion with example.**

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

### **7. What is Module in Python? Give detailed description of it with example.**

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
