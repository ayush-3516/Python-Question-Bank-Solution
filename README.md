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
    - [13. Differentiate Strings, Tuples, Lists and Dictionaries.](#13-differentiate-between-strings-tuples-lists-and-dictionaries)
    - [14. List out operations on Strings, Tuples, Lists and Dictionaries.](#14-list-out-operations-on-strings-tuples-lists-and-dictionaries)
    - [15. What is Cloning? Describe methods to overcome it.](#15-what-is-cloning-describe-methods-to-overcome-it)
    - [16. Explain Membership Operator with example.](#16-explain-membership-operator-with-example)
- [Unit - 2]()
    - [17. List and explain types of inheritance in python with example.]()
    - [18. Explain Data Abstraction/Data Hiding]()
    - [19. Explain isinstance() method.]()
    - [20. Explain Method overriding.]()
    - [21. Explain issubclass() method.]()
    - [22. Discuss Encapsulation.]()
    - [23. Implementation of linear search/binary search(recursive/non-recursive)]()
    - [24. Explain Wrapper Function.]()
    - [25. Write a code to implement divide and conquer/merge sort/selection sort.]()
    - [26. Write a code to implement tim sort.]()
    - [27. Lisked list concept in python.]()
    - [28. Describe methods of regular expressions(RegEx).]()
    - [29. Types of Pattern Formation in Python RegEx.]()
    - [30. Expressions based RegEx.]()
    - [31. Discuss Thread Control Block(TCB).]()
    - [32. Thread Control Methods.]()
    - [33. Multithreading in Python.]()
    - [34. Multithreading with lock() synchronization.]()
    - [35. Client Server Chat Applicatios and required commands.]()
- [Unit - 3]()
    - [36. Describe methods to create an array using numpy.]()
    - [37. When to use reshape method in numpy? Explain with example.]()
    - [38. Apply Arithmetic operators, relational operators and logical operators on vector using numpy.]()
    - [39. Explain compount condition in numpy.]()
    - [40. How to create an alias of an array using numpy?]()
    - [41. Briefly explain matrix module.]()
    - [42. Explain generation of random number, all zero valued matrices, all ones valued matrices, identity matrix.]()
    - [43. Draw plot for given data using Pylab/matplotlib and numpy.]()
    - [44. Implementation of client and server in context of chat application.]()
    - [45. List and explain methods supported by tkinter to place/arrange various widgets in window.]()
    - [46. Explain steps to create widgets. Write python program to display a label on clicking a button using tkinter.(any widgets)]()
    - [47. Significance of Intvar class in tkinter.]()
    - [48. Write a code to draw rectangle with border color of blue and inner filling of color yellow using turtle.]()
    - [49. List and explain methods supported by tutle module.]()
- [Unit - 4]()
    - [50.Explain DataFrames/Series with row header and column header in pandas.]()
    - [51. How to import external files(Example: txt, excel, csv) using pandas?]()
    - [52. Discuss data retrieval methods of pandas.]()
    - [53. How to search specific value based on certain condition or combination of conditions in pandas.]()
    - [54. Explain groupby and sort_values in pandas.]()
    - [55. Draw plot for given data using Pylab/matplotlib and pandas.]()
    - [56. Describe libraries and methods used in flask.]()
    - [57. How to use Cookies and flash messages in flask.]()
    - [58. List and explain flask extensions.]()
    - [59. How to embed HTML templates in flask?]()
    - [60. Explain tensorflow architecture and components.]()
    
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

1. Lists (`list`):

Lists are ordered collections of items, and their elements can be modified, added, or removed after creation.
```python
my_list = [1, 2, 3]
my_list[0] = 5  # Modifying an element
my_list.append(4)  # Adding an element
```

2. Dictionaries(`dict`):

Dictionaries are collections of key-value pairs, and their keys and values can be modified, added, or removed.
```python
my_dict = {'name': 'Alice', 'age': 30}
my_dict['age'] = 31  # Modifying a value
my_dict['city'] = 'New York'  # Adding a key-value pair
```

3. Sets(`set`):

Sets are unordered collections of unique elements, and their elements can be modified or added.
```python
my_set = {1, 2, 3}
my_set.add(4)  # Adding an element
```

### **13. Differentiate between Strings, Tuples, Lists, and Dictionaries.**

**Strings (`str`)**
- Description:
    - A string is an ordered collection of characters.
    - Immutable: Strings cannot be modified once created; you can only create new strings.
- Example:
```python
my_str = "Hello, World!"
```
- Properties:
    - Ordered: Characters have a specific order and can be accessed by index.
    - Immutable: You cannot modify a string in-place.
    - Iterable: You can iterate over the characters in a string.

**Tuples (`tuple`)**
- Description:
    - A tuple is an ordered collection of elements, which can be of any data type.
    - Immutable: Tuples cannot be modified once created; you can only create new tuples.
- Example:
```python
my_tuple = (1, "Alice", 3.14)
```
- Properties:
    - Ordered: Elements have a specific order and can be accessed by index.
    - Immutable: You cannot modify a tuple in-place.
    - Iterable: You can iterate over the elements in a tuple.

**Lists (`list`)**
- Description:
    - A list is an ordered collection of elements, which can be of any data type.
    - Mutable: Lists can be modified by adding, removing, or changing elements in-place.
- Example:
```python
my_list = [1, "Alice", 3.14]
```
- Properties:
    - Ordered: Elements have a specific order and can be accessed by index.
    - Mutable: You can modify a list in-place by adding, removing, or changing elements.
    - Iterable: You can iterate over the elements in a list.

**Dictionaries (`dict`)**
- Description:
    - A dictionary is an unordered collection of key-value pairs.
    - Mutable: Dictionaries can be modified by adding, removing, or changing key-value pairs.
- Example:
```python
my_dict = {"name": "Alice", "age": 30}
```
- Properties:
    - Unordered: Key-value pairs do not have a specific order and cannot be accessed by index.
    - Mutable: You can modify a dictionary in-place by adding, removing, or changing key-value pairs.
    - Iterable: You can iterate over the keys, values, or key-value pairs in a dictionary.

### **14. List out operations on Strings, Tuples, Lists and Dictionaries.**

**Strings (`str`)**

1. Concatenation:

Joining two or more strings together.

Example:
```python
str1 = "Hello"
str2 = "World"
result = str1 + " " + str2  # Output: "Hello World"
```

2. Indexing:

Accessing elements in a tuple using their indices.

Example:
```python
my_str = "Python"
print(my_str[0])  # Output: 'P'
```

3. Slicing:

Extracting a portion of the string.

Example:
```python
my_str = "Hello, World!"
print(my_str[7:12])  # Output: "World"
```

4. Length:

Getting the length of the string.

Example:
```python
my_str = "Hello"
print(len(my_str))  # Output: 5
```

5. Membership:

Checking if a substring is present in the string.

Example:
```python
my_str = "Hello, World!"
print("World" in my_str)  # Output: True
```

6. Conversion:

Converting a string to uppercase, lowercase, or titlecase.

Example:
```python
my_str = "hello"
print(my_str.upper())  # Output: "HELLO"
print(my_str.lower())  # Output: "hello"
print(my_str.title())  # Output: "Hello"
```

7. Splitting and Joining:

Splitting a string into a list of substrings or joining a list of strings into a single string.

Example:
```python
my_str = "apple,banana,cherry"
split_result = my_str.split(",")  # Output: ['apple', 'banana', 'cherry']
join_result = "-".join(split_result)  # Output: "apple-banana-cherry"
```

**Tuples (`tuple`)**

1. Indexing:

Accessing elements in a tuple using their indices.

Example:
```python
my_tuple = (10, 20, 30)
print(my_tuple[0])  # Output: 10
```

2. Slicing:

Extracting a portion of the tuple.

Example:
```python
my_tuple = (1, 2, 3, 4, 5)
print(my_tuple[1:4])  # Output: (2, 3, 4)
```

3. Length:

Getting the length of a tuple(number of elements).

Example:
```python
my_tuple = (1, 2, 3)
print(len(my_tuple))  # Output: 3
```

4. Membership:

Checking in an element is present in the tuple.

Example:
```python
my_tuple = (10, 20, 30)
print(20 in my_tuple)  # Output: True
```

**Lists (`list`)**

1. Append and Extend:

Adding elements to a list.

Example:
```python
my_list = [1, 2, 3]
my_list.append(4)  # Appends a single element
my_list.extend([5, 6, 7])  # Extends the list with another list
```

2. Insert:

Inserting an element at a specific position in the list.

Example:
```python
my_list = [1, 2, 3]
my_list.insert(1, 10)  # Inserts 10 at index 1
```

3. Remove and Pop:

Removing elements from the list.

Example:
```python
my_list = [10, 20, 30]
my_list.remove(20)  # Removes the specified element
my_list.pop(0)  # Removes and returns the element at the specified index
```

4. Index and Count:

Finding the index of an element and counting occurrences.

Example:
```python
my_list = [1, 2, 3, 2]
print(my_list.index(2))  # Output: 1 (index of the first occurrence of 2)
print(my_list.count(2))  # Output: 2 (number of occurrences of 2)
```

5. Sorting and Reversing:

Sorting and Reversing the elements in the list.

Example:
```python
my_list = [5, 3, 8, 1]
my_list.sort()  # Sorts the list in-place
my_list.reverse()  # Reverses the list in-place
```

**Dictionaries (`dict`)**

1. Accessing Values:

Accessing values in a dictionary using keys.

Example:
```python
my_dict = {"name": "Alice", "age": 30}
print(my_dict["name"])  # Output: "Alice"
```

2. Keys, Values, and Items:

Getting keys, values, and key-value pairs from a dictionary.

Example:
```python
my_dict = {"name": "Alice", "age": 30}
print(my_dict.keys())  # Output: dict_keys(['name', 'age'])
print(my_dict.values())  # Output: dict_values(['Alice', 30])
print(my_dict.items())  # Output: dict_items([('name', 'Alice'), ('age', 30)])
```

3. Adding, Modifying, and Removing Items:

Adding, Modifying and Removing items in the dictionary.

Example:
```python
my_dict = {"name": "Alice", "age": 30}
my_dict["city"] = "New York"  # Adding a new key-value pair
my_dict["age"] = 31  # Modifying an existing value
del my_dict["name"]  # Removing a key-value pair
```

4. Membership:

Checking if a key is present in the dictionary.

Example:
```python
my_dict = {"name": "Alice", "age": 30}
print("name" in my_dict)  # Output: True
```

### **15. What is Cloning? Describe methods to overcome it.**

Cloning, in the context of data structures and objects, refers to the process of creating a copy of an existing object or data structure. When you clone an object, you create a new object that has the same content (values) as the original, but is a distinct entity in memory. Cloning is important to avoid unintended modifications to the original object when working with its copy.

In Python, the concept of cloning is relevant mainly for mutable objects like lists, dictionaries, and custom objects, since they can be modified in-place.

**Methods to Overcome Cloning Issues:**
1. Shallow Copy:

- A shallow copy creates a new object that is a duplicate of the original object, but it doesn't create copies of the objects inside the original object (e.g., elements of a list).
- Use the copy() method for lists, dictionaries, and other mutable objects to create a shallow copy.
- Shallow copy can still have issues if the original object contains mutable objects.

```python
import copy

original_list = [1, [2, 3]]
shallow_copy = copy.copy(original_list)

shallow_copy[1][0] = 5  # This will affect the original list too
```

2. Deep Copy:

- A deep copy creates a new object that is a duplicate of the original object, including all objects inside it (recursively).
- Use the `deepcopy()` method from the copy module for creating deep copies.

```python
import copy

original_list = [1, [2, 3]]
deep_copy = copy.deepcopy(original_list)

deep_copy[1][0] = 5  # This won't affect the original list
```

3. Slice Operator (for Lists):

- Using the slice operator ([:]) can create a shallow copy of a list.
- This works specifically for lists and provides a simple way to create a new list with the same elements.

```python
original_list = [1, 2, 3]
shallow_copy = original_list[:]

shallow_copy[0] = 5  # This won't affect the original list
```

4. Constructors(for Lists and Dictionaries):

- Creating a new list or dictionary using the constructor of the respective type can also achieve a shallow copy.

```python
original_list = [1, 2, 3]
shallow_copy = list(original_list)  # Shallow copy using list constructor

original_dict = {"a": 1, "b": 2}
shallow_copy_dict = dict(original_dict)  # Shallow copy using dict constructor
```

5. Custom Cloning(for Custom Objects):

- Implement a custom method within your class to create a new instance and copy relevant attributes or data.

```python
class CustomObject:
    def __init__(self, value):
        self.value = value

    def clone(self):
        return CustomObject(self.value)

original_obj = CustomObject(42)
cloned_obj = original_obj.clone()
```

### **16. Explain Membership Operator with example.**

Membership operators in Python are used to test for membership in a sequence, such as strings, lists, tuples, or dictionaries. There are two membership operators: `in` and `not in`.

`in` Operator
The `in` operator checks if a value exists in a sequence. It returns `True` if the value is present and `False` otherwise.

Syntax:

```python
value in sequence
```

Example:

```python
my_list = [1, 2, 3, 4, 5]

print(3 in my_list)  # Output: True
print(6 in my_list)  # Output: False
```

not in Operator
The not in operator checks if a value does not exist in a sequence. It returns True if the value is not present and False otherwise.

Syntax:not in Operator
The not in operator checks if a value does not exist in a sequence. It returns True if the value is not present and False otherwise.

Syntax:
```python
value not in sequence
```

Example:

```python
my_str = "Hello, World!"

print('H' not in my_str)  # Output: False
print('x' not in my_str)  # Output: True
```

## Unit - 2

### **17. List and explain types of Inheritance in python with example.**

**Single Inheritance** Single inheritance allows a derivate class to inherit properties of one parent class, and this allows code reuse and the introduction of additional features in existing code.

```python
class Parent1:  
    def func_1(self):  
        print ("This function is defined inside the parent class.")  
  
class Child1(Parent1):  
    def func_2(self):  
        print ("This function is defined inside the child class.")  
  
# Driver's code  
object = Child1()  
object.func_1()  
object.func_2() 
```
Output:
```
This function is defined inside the parent class.
This function is defined inside the child class.
```

**Multiple Inheritance** If a class is able to be created from multiple base classes, this kind of Inheritance is known as multiple Inheritance. When there is multiple Inheritance, each of the attributes that are present in the classes of the base has been passed on to the class that is derived from it.

```python
class Mother1:  
    mothername1 = ""  
    def mother1(self):  
        print(self.mothername1)  
  
class Father1:  
    fathername1 = ""  
    def father1(self):  
        print(self.fathername1)  
  
class Son1(Mother1, Father1):  
    def parents1(self):  
        print ("Father name is :", self.fathername1)  
        print ("Mother name is :", self.mothername1)  
  
s1 = Son1()  
s1.fathername1 = "Rajesh"  
s1.mothername1 = "Shreya"  
s1.parents1() 
```
Output:
```
Father name is: Rajesh
Mother name is: Shreya
```

**Multilevel inheritance**, the features that are part of the original class, as well as the class that is derived from it, are passed on to the new class. It is similar to a relationship involving grandparents and children.

```python
class Grandfather1:  
  
    def __init__(self, grandfathername1):  
        self.grandfathername1 = grandfathername1  
  
class Father1(Grandfather1):  
    def __init__(self, fathername1, grandfathername1):  
        self.fathername1 = fathername1  
  
        Grandfather1.__init__(self, grandfathername1)  
  
class Son1(Father1):  
    def __init__(self,sonname1, fathername1, grandfathername1):  
        self.sonname1 = sonname1  
  
        Father1.__init__(self, fathername1, grandfathername1)  
  
    def print_name(self):  
        print('Grandfather name is :', self.grandfathername1)  
        print("Father name is :", self.fathername1)  
        print("Son name is :", self.sonname1)  
  
s1 = Son1('John', 'John Jr', 'John Jr Jr')  
print (s1.grandfathername1)  
s1.print_name() 
```
Output:
```
John Jr Jr
Grandfather name is : John Jr Jr
Father name is : John Jr
Son name is : John
```

**Hierarchical Inheritance** If multiple derived classes are created from the same base, this kind of Inheritance is known as hierarchical inheritance. In this instance, we have two base classes as a parent (base) class as well as two children (derived) classes.

```python
class Parent1:  
    def func_1(self):  
        print ("This function is defined inside the parent class.")  
  
class Child_1(Parent1):  
    def func_2(self):  
        print ("This function is defined inside the child 1.")  
  
class Child_2(Parent1):  
    def func_3(self):  
        print ("This function is defined inside the child 2.")  
  
object1 = Child_1()  
object2 = Child_2()  
object1.func_1()  
object1.func_2()  
object2.func_1()  
object2.func_3() 
```
Output:
```
This function is defined inside the parent class.
This function is defined inside the child 1.
This function is defined inside the parent class.
This function is defined inside the child 2.
```

### **18. Explain Data Abstraction/Data Hiding.**

Data abstraction that hides complex implementation details while exposing only essential information and functionalities to users. In Python, we can achieve data abstraction by using abstract classes and abstract classes can be created using abc (abstract base class) module and abstractmethod of abc module.
