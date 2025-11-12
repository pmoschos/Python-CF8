# 🧮 Python String Formatting and Math Module

This lesson explores how to format strings in Python for readable output and how to use the `math` module for common mathematical operations. You’ll learn to create clear, informative print statements and perform calculations using Python’s standard library.

---

## 1. Learning Objectives

- Understand and apply different string formatting techniques in Python.
- Use f-strings and the `format()` method for dynamic, readable output.
- Import and utilize the Python `math` module for mathematical operations.
- Apply mathematical functions like `sqrt`, `pow`, `ceil`, `floor`, and `pi`.
- Combine string formatting with math operations for practical programs.

---

## 2. Prerequisites

- Basic Python syntax (variables, functions, print statements).
- Familiarity with numeric data types (int, float).
- Understanding of importing modules in Python.

---

## 3. Key Concepts

- **String Formatting**: Methods to insert variable values into strings for output.
- **f-string**: String literals prefixed with `f` that allow embedded expressions (Python 3.6+).
- **`format()` Method**: A string method to substitute values into placeholders `{}`.
- **Math Module (`math`)**: A standard Python library providing mathematical functions.
- **`math.sqrt(x)`**: Returns the square root of `x`.
- **`math.pow(x, y)`**: Returns `x` raised to the power of `y`.
- **`math.ceil(x)`**: Returns the smallest integer greater than or equal to `x`.
- **`math.floor(x)`**: Returns the largest integer less than or equal to `x`.
- **`math.pi`**: The mathematical constant π (pi).

---

## 4. Lecture Outline

### 0:00–0:05 — Introduction
- Why is readable output important?
- Motivation: Calculating and displaying results clearly.

### 0:05–0:15 — String Formatting in Python
- Old-style: `%` operator (brief mention)
- Modern methods:
  - f-strings: `f"Value is {value}"`
  - `str.format()`: `"Value is {}".format(value)`
- Examples:
  - Printing variables
  - Formatting numbers (decimals, width)

### 0:15–0:25 — The Math Module
- Importing the module: `import math`
- Common functions:
  - `math.sqrt()`, `math.pow()`
  - `math.ceil()`, `math.floor()`
  - `math.pi`
- Examples: Calculating square roots, powers, rounding

### 0:25–0:30 — Combining Formatting and Math
- Displaying results with context:
  - "The square root of 2 is 1.414..."
  - Formatting decimals to 2 places
- Q&A and summary

---

## 5. Code Demos

```python
import math  # Import the math module to access mathematical constants and functions

# Define string and integer variables
name = "Alice"
age = 20

# Print a simple string
print("CF")
# Print the mathematical constant PI from the math module
print("PI =", math.pi)

# Demonstrate string concatenation
print("String Concatenation")
# This line would cause a TypeError because you cannot concatenate string and integer directly
# print(name + " is" + age + " years old.")  # Incorrect way, commented out
print(name + " is " + str(age) + " years old.")  # Correct by converting age to a string
print("-------------------------")

# Demonstrate old Python 2 style string formatting using the % operator
print("Python 2 style")
print("PI = %6.2f" % math.pi)  # Format PI to two decimal places with padding
print("%s is %d years old" % (name, age))  # Use placeholders for string and integer
print("-------------------------")

# Demonstrate Python 3 style string formatting using the str.format() method
print("Python 3 style using string format")
print("Age is {0:2d}".format(age))  # Format age with 2-digit padding
print("PI = {0:.3f}".format(math.pi))  # Format PI to three decimal places
# Explanation of the '0' in format: It refers to the first argument passed to format()
print("PI = {0:.3f} and age = {1}".format(math.pi, age))  # Multiple placeholders
print("-------------------------")

# Print combining text and variables using format and specifying the print end character
print("{0} is {1}".format(name, age), end=" ")
print("years old.")

# Using string formatting for alignment and padding
print("{0:*^10}:{1:>20}".format(name, age))  # Center name with asterisks, right-align age
print("{0:*^10}:{1:<20}".format(name, age), end="|")  # Left-align age, end print with '|'
print("-------------------------")

# Demonstrate modern Python 3 style string interpolation using f-strings
print("Python 3 style using f-strings")
print(f"{name} is {age} years old.")  # Embed expressions inside string literals directly

# Some extra information about math functions
print(math.sqrt(16))      # Output: 4.0
print(math.pow(2, 5))     # Output: 32.0
print(math.ceil(2.3))     # Output: 3
print(math.floor(2.7))    # Output: 2
print(math.pi)            # Output: 3.141592653589793

# Combining math and formatting
radius = 3
area = math.pi * math.pow(radius, 2)
print(f"Circle area with radius {radius}: {area:.2f}")  # Output: Circle area with radius 3: 28.27
```

---

## 6. Exercises

### 1. (Level 1, MCQ)
Which of the following will print the value of `x = 5` as "The value is 5"?

a) `print("The value is x")`  
b) `print(f"The value is {x}")`  
c) `print("The value is {}".format(x))`  
d) Both b) and c)

<details>
<summary>Solution</summary>

**Answer:** d) Both b) and c)
</details>

---

### 2. (Level 1, Short Answer)
What is the output of the following code?

```python
import math
print(math.ceil(4.2))
```

<details>
<summary>Solution</summary>

**Output:** `5`
</details>

---

### 3. (Level 2, Coding)
Write a Python statement that prints the square root of 50 rounded to 3 decimal places, using an f-string.

<details>
<summary>Solution</summary>

```python
import math
print(f"The square root of 50 is {math.sqrt(50):.3f}")
# Output: The square root of 50 is 7.071
```
</details>

---

### 4. (Level 2, Coding)
Given `radius = 5`, use the `math` module and string formatting to print:  
"The area of a circle with radius 5 is 78.54"

<details>
<summary>Solution</summary>

```python
import math
radius = 5
area = math.pi * math.pow(radius, 2)
print(f"The area of a circle with radius {radius} is {area:.2f}")
# Output: The area of a circle with radius 5 is 78.54
```
</details>

---

### 5. (Level 3, Coding) - We will learn about functions in future chapter!
Write a function that takes a number and prints both its square and its square root, each rounded to 2 decimal places, using formatted output.

Example:  
`print_square_and_root(7)`  
should print:  
"Square: 49.00, Square root: 2.65"

<details>
<summary>Solution</summary>

```python
import math

def print_square_and_root(n):
    square = math.pow(n, 2)
    root = math.sqrt(n)
    print(f"Square: {square:.2f}, Square root: {root:.2f}")

# Example usage:
print_square_and_root(7)
# Output: Square: 49.00, Square root: 2.65
```
</details>

---

## 7. Further Reading

- [Python Official Documentation: String Formatting](https://docs.python.org/3/library/string.html#format-string-syntax)
- [Python Official Documentation: math Module](https://docs.python.org/3/library/math.html)

---

## 📢 Stay Updated
Be sure to ⭐ this repository to stay updated with new examples and enhancements!

## 📄 License
🔐 This project is protected under the [MIT License](https://mit-license.org/).


## Contact 📧
Panagiotis Moschos - pan.moschos86@gmail.com

🔗 *Note: This is a Python script and requires a Python interpreter to run.*

---
<h1 align="center">Happy Coding 👨‍💻</h1>

<p align="center">
  Made with ❤️ by <a href="https://www.linkedin.com/in/panagiotis-moschos">Panagiotis Moschos</a> (<a href="https://github.com/pmoschos">GitHub</a>)
</p>