## Assignment: Introduction to Python

### 1. Python Basics

**What is Python?**
Python is a high-level, interpreted programming language known for its simplicity and readability. It supports multiple programming paradigms, including procedural, object-oriented, and functional programming.

**Key Features of Python:**
- **Easy to Learn and Use:** Python's syntax is clear and concise, making it accessible for beginners.
- **Interpreted Language:** Python code is executed line by line, which makes debugging easier.
- **Cross-Platform:** Python runs on various operating systems, including Windows, macOS, and Linux.
- **Extensive Standard Library:** Python's standard library offers modules and functions for various tasks, from web development to data analysis.
- **Community Support:** Python has a large and active community that contributes to its development and provides support.

**Use Cases of Python:**
- **Web Development:** Frameworks like Django and Flask.
- **Data Analysis and Machine Learning:** Libraries like pandas, NumPy, and scikit-learn.
- **Scripting and Automation:** Automating repetitive tasks.
- **Scientific Computing:** Libraries like SciPy.
- **Game Development:** Libraries like Pygame.

### 2. Installing Python

**Steps to Install Python on Windows:**
1. **Download the Installer:**
   - Go to the official [Python website](https://www.python.org/).
   - Download the latest version for Windows.

2. **Run the Installer:**
   - Open the downloaded installer.
   - Check the box “Add Python to PATH.”
   - Click “Install Now.”

3. **Verify the Installation:**
   - Open Command Prompt.
   - Type `python --version` and press Enter. You should see the installed Python version.

**Setting Up a Virtual Environment:**
1. **Open Command Prompt.**
2. **Navigate to your project directory.**
3. **Create a virtual environment:**
    python -m venv myenv
 
4. **Activate the virtual environment:**
   - On Windows:
    myenv\Scripts\activate
    
   - On macOS/Linux:
    source myenv/bin/activate
   
### 3. Python Syntax and Semantics

**Simple Python Program:**
print("Hello, World!")

**Explanation:**
- `print`: A built-in function used to output text to the console.
- `"Hello, World!"`: A string, which is a sequence of characters enclosed in quotes.

### 4. Data Types and Variables

**Basic Data Types in Python:**
- **int:** Integer numbers (e.g., 5)
- **float:** Floating-point numbers (e.g., 3.14)
- **str:** Strings (e.g., "hello")
- **bool:** Boolean values (True or False)
- **list:** Ordered collection of items (e.g., [1, 2, 3])
- **dict:** Key-value pairs (e.g., {"key": "value"})

**Script Demonstrating Variables:**
Integer
age = 25

Float
height = 5.9

String
name = "Alice"

Boolean
is_student = True

List
numbers = [1, 2, 3, 4, 5]

Dictionary
person = {"name": "Alice", "age": 25}

print(age, height, name, is_student, numbers, person)

### 5. Control Structures

**Conditional Statements:**
x = 10
if x > 5:
    print("x is greater than 5")
else:
    print("x is 5 or less")

**Loops:**
For loop
for i in range(5):
    print(i)

While loop
count = 0
while count < 5:
    print(count)
    count += 1

### 6. Functions in Python

**What are Functions?**
Functions are reusable blocks of code that perform a specific task. They help in organizing code, reducing redundancy, and improving readability.

**Function Example:**
def add(a, b):
    return a + b

# Calling the function
result = add(5, 3)
print(result)  # Output: 8

### 7. Lists and Dictionaries

**Differences:**
- **Lists:** Ordered collection of items, accessible by index.
- **Dictionaries:** Unordered collection of key-value pairs, accessible by key.

**Script Demonstrating Lists and Dictionaries:**
List
numbers = [1, 2, 3, 4, 5]
numbers.append(6)
print(numbers)

Dictionary
person = {"name": "Alice", "age": 25}
person["city"] = "New York"
print(person)

### 8. Exception Handling

**What is Exception Handling?**
Exception handling is used to manage errors gracefully without crashing the program.

**Example:**
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero")
finally:
    print("Execution complete")

### 9. Modules and Packages

**Modules and Packages:**
- **Module:** A file containing Python code, which can be imported and used in other scripts.
- **Package:** A directory containing multiple modules.

**Importing and Using a Module:**
import math

result = math.sqrt(16)
print(result) 

### 10. File I/O

**Reading from a File:**
with open("example.txt", "r") as file:
    content = file.read()
    print(content)

**Writing to a File:**
lines = ["First line", "Second line", "Third line"]

with open("output.txt", "w") as file:
    for line in lines:
        file.write(line + "\n")
