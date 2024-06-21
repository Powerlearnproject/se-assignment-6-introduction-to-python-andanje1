[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15309454&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
   Python is a high-level, interpreted programming language known for its simplicity and readability. Some key features that make Python popular include:

Easy-to-read syntax: Python emphasizes readability with its clear and expressive syntax.
Versatility: Python is suitable for a wide range of applications, from web development to scientific computing and data analysis.
Large standard library: Python comes with a vast collection of libraries and modules that simplify complex tasks.
Community and support: Python has a large and active community, offering extensive documentation, tutorials, and support.
Use cases: Python is effective in:

Web development (Django, Flask)
Data analysis and visualization (Pandas, Matplotlib)
Machine learning and AI (TensorFlow, PyTorch)
Scripting and automation
Scientific computing (NumPy, SciPy)

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   Here are the general steps:

Download Python: Visit the official Python website and download the installer suitable for your operating system.

Install Python:

Windows: Run the installer, select "Add Python to PATH," and follow the prompts.
macOS: Run the installer package and follow the instructions.
Linux: Python is usually pre-installed. Use your package manager to install it if not (sudo apt-get install python3 for Debian-based, sudo yum install python3 for Red Hat-based).
Verify Installation: Open a terminal (command prompt on Windows) and type python --version (or python3 --version on some systems) to check if Python is installed and the version.

Set Up a Virtual Environment (optional but recommended):

Install virtualenv if not already installed: pip install virtualenv.
Create a virtual environment: virtualenv myenv.
Activate the virtual environment:
Windows: myenv\Scripts\activate
macOS/Linux: source myenv/bin/activate

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
   Here's the program:
   # Simple Hello, World! program
print("Hello, World!")
Explanation:

print(): A built-in function that outputs to the console.
"Hello, World!": A string literal enclosed in double quotes.
#: Denotes a comment in Python.


4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
   : Basic data types in Python include:

int: Integer numbers (5, -3, 1000)
float: Floating-point numbers (3.14, 2.718)
str: Strings of characters ("hello", 'world')
bool: Boolean values (True, False)
list: Ordered collection of items ([1, 2, 3])
tuple: Immutable ordered collection ((1, 2, 3))
dict: Collection of key-value pairs ({'name': 'Alice', 'age': 30})

Example script demonstrating variables:
# Variables of different types
x = 5           # int
y = 3.14        # float
name = "Alice"  # str
is_student = True  # bool

# Lists
numbers = [1, 2, 3, 4, 5]

# Dictionary
person = {'name': 'Bob', 'age': 25, 'is_student': False}

# Accessing variables
print(x)
print(name)
print(numbers)
print(person)


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
   A: Conditional statements and loops control the flow of execution in Python:

if-else statement:

# Example of an if-else statement
age = 20

if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")

for loop:

# Example of a for loop
numbers = [1, 2, 3, 4, 5]

for num in numbers:
    print(num)


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   Functions in Python are blocks of reusable code designed to perform a specific task. They promote code reusability, modularity, and easier debugging. ExFunctions in Python are blocks of reusable code designed to perform a specific task. They promote code reusability, modularity, and easier debugging. Example of a function:

# Function to calculate sum of two numbers
def sum_numbers(a, b):
    return a + b

# Calling the function
result = sum_numbers(3, 5)
print("Sum:", result)


7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
   Lists are ordered collections of items accessed by index, while dictionaries are unordered collections of key-value pairs accessed by key. Example script:
   # List of numbers
numbers = [1, 2, 3, 4, 5]

# Dictionary of key-value pairs
person = {'name': 'Alice', 'age': 30, 'city': 'New York'}

# Accessing elements
print(numbers[0])          # Accessing first element of list
print(person['name'])      # Accessing value by key in dictionary

# Adding new elements
numbers.append(6)          # Adding a number to the list
person['job'] = 'Engineer' # Adding a new key-value pair to the dictionary

# Iterating through elements
for num in numbers:
    print(num)

for key, value in person.items():
    print(key, ":", value)


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
   Exception handling allows you to handle errors gracefully. 

   # Example of exception handling
try:
    num = int(input("Enter a number: "))
    result = 10 / num
    print("Result:", result)
except ZeroDivisionError:
    print("Error: Cannot divide by zero!")
except ValueError:
    print("Error: Invalid input. Please enter a number.")
finally:
    print("Execution completed.")


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
   Modules are files containing Python code, and packages are directories of modules. You can import modules using import keyword. 

   # Example of importing and using a module
import math

# Using math module
print("Pi:", math.pi)
print("Square root of 16:", math.sqrt(16))



10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
    # Reading from a file
file_path = 'sample.txt'

with open(file_path, 'r') as file:
    content = file.read()
    print("File content:")
    print(content)

# Writing to a file
output_file = 'output.txt'
lines_to_write = ["First line\n", "Second line\n", "Third line\n"]

with open(output_file, 'w') as file:
    file.writelines(lines_to_write)

print(f"Lines written to {output_file}")

References:

Python documentation index (2022) Python.org. Available at: https://www.python.org/doc/essays/ (Accessed: 21 June 2024). 

input and output (2024) Python documentation. Available at: https://docs.python.org/3/tutorial/inputoutput.html#reading-and-writing-files (Accessed: 21 June 2024). 

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


