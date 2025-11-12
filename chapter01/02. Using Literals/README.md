# 🟦 Python Variables and Data Types

A foundational lesson on how Python uses variables and data types, focusing on literals and their assignment, as referenced in [python-CF7/chapter01/02. Using Literals](https://github.com/pmoschos/python-CF7/tree/main/chapter01/02.%20Using%20Literals).

---

## 1. Learning Objectives

- Understand what variables are and how to assign values to them in Python.
- Identify and use Python's core data types: integers, floats, strings, and booleans.
- Recognize and use literals for each data type.
- Predict the type and value of variables after assignment.
- Use the `type()` function to inspect variable types.
- Apply best practices for naming variables.

---

## 2. Prerequisites

- Familiarity with basic Python syntax (how to run Python code).
- Understanding of what a programming variable is (in any language).
- Ability to use a Python interpreter or IDE.

---

## 3. Key Concepts

- **Variable**: A named reference to a value stored in memory.
- **Assignment (`=`)**: The operation of storing a value in a variable.
- **Literal**: A direct value in code (e.g., `42`, `3.14`, `'hello'`, `True`).
- **Data Type**: The kind of value a variable holds (e.g., `int`, `float`, `str`, `bool`).
- **Integer (`int`)**: Whole numbers, e.g., `5`, `-3`.
- **Float (`float`)**: Numbers with decimals, e.g., `2.5`, `-0.1`.
- **String (`str`)**: Text enclosed in quotes, e.g., `"Python"`, `'42'`.
- **Boolean (`bool`)**: Logical values: `True` or `False`.
- **`type()`**: Built-in function to check the data type of a variable.

---

## 4. Lecture Outline

### 0:00–0:05 — Introduction to Variables
- What is a variable?
- Why do we need variables in programming?
- Syntax: `variable_name = value`
- Example: `age = 25`

### 0:05–0:12 — Python Data Types and Literals
- Overview of core data types: `int`, `float`, `str`, `bool`
- What is a literal? Examples for each type:
  - Integer: `7`
  - Float: `3.14`
  - String: `'hello'`, `"world"`
  - Boolean: `True`, `False`
- Demo: Assigning literals to variables

### 0:12–0:18 — Inspecting Variable Types
- Using `type()` to check a variable's data type
- Example: `type(age)`
- Predicting types before running code

### 0:18–0:23 — Variable Naming and Best Practices
- Rules: start with letter/underscore, no spaces, case-sensitive
- Good vs. bad variable names
- Convention: `snake_case`

### 0:23–0:28 — Type Conversion (Casting)
- Converting between types: `int()`, `float()`, `str()`, `bool()`
- Example: `int("42")`, `float(5)`, `str(3.14)`, `bool(0)`
- When and why to convert types

### 0:28–0:30 — Q&A and Recap
- Review: variables, types, literals, naming, type checking

---

## 5. Code Demos

```python
# Initialize three integer variables in different number systems
num1 = 10           # Decimal format
num2 = 0b1010       # Binary format
num3 = 0x000A       # Hexadecimal format

# Initialize string variables in various quotation styles
str1 = 'CF'         # Single quotes for short strings
str2 = "CF"         # Double quotes, interchangeable with single quotes for strings
str3 = 'Cod\
ing'                # Line continuation character used to extend the string across the newline

# Multi-line string using triple single quotes
str4 = '''Hello
Coding
Factory'''

# Multi-line string using triple double quotes
str5 = """Hello
again!
"""

# Boolean variable initialized as True
my_bool = True

# Print the initialized variables to observe their values and types
print(num1, num2, num3, str1, str2, str3, my_bool)
print("----------------")

# Display text to categorize output
print("Types:")

# Print the data types of each variable to show the distinction between them
print(type(num1))     # Should show <class 'int'>
print(type(num2))     # Should show <class 'int'>
print(type(num3))     # Should show <class 'int'>
print(type(str1))     # Should show <class 'str'>
print(type(str2))     # Should show <class 'str'>
print(type(str3))     # Should show <class 'str'>
print(type(str4))     # Should show <class 'str'>
print(type(str5))     # Should show <class 'str'>
print(type(my_bool))  # Should show <class 'bool'>

# Assigning literals to variables
age = 30         # int literal
height = 1.75    # float literal
name = "Alice"   # string literal
is_student = True  # boolean literal

# Checking types
print(type(age))        # <class 'int'>
print(type(height))     # <class 'float'>
print(type(name))       # <class 'str'>
print(type(is_student)) # <class 'bool'>

# Type conversion (casting)
age_str = str(age)      # Converts int to string
print(age_str, type(age_str))  # '30' <class 'str'>

height_int = int(height)  # Converts float to int (truncates decimals)
print(height_int)         # 1

# Variable naming
user_score = 100
_user2 = "Bob"
# Invalid: 2user = "Eve"  # SyntaxError
```

---

## 6. Exercises

### 1. (Level 1, MCQ)
Which of the following is a valid variable assignment in Python?
- a) `2name = "Bob"`
- b) `user-name = "Alice"`
- c) `user_name = "Eve"`
- d) `user name = "Sam"`

<details>
<summary>Solution</summary>

**Answer:** c) `user_name = "Eve"`
</details>

---

### 2. (Level 1, Short Answer)
What is the output of the following code?

```python
x = 3.5
print(type(x))
```

<details>
<summary>Solution</summary>

**Output:** `<class 'float'>`
</details>

---

### 3. (Level 2, Coding)
Assign the integer literal `42` to a variable named `answer`. Print its type.

```python
# Your code here
```

<details>
<summary>Solution</summary>

```python
answer = 42
print(type(answer))  # <class 'int'>
```
</details>

---

### 4. (Level 2, Coding)
Given the string variable `s = "123"`, convert it to an integer and add 7. Print the result.

```python
s = "123"
# Your code here
```

<details>
<summary>Solution</summary>

```python
s = "123"
result = int(s) + 7
print(result)  # 130
```
</details>

---

### 5. (Level 3, Coding)
Write a program that assigns a value to a variable, prints its type, then converts it to a different type and prints the new type. Use a float-to-string conversion as your example.

```python
# Your code here
```

<details>
<summary>Solution</summary>

```python
value = 5.67
print(type(value))       # <class 'float'>
value_str = str(value)
print(type(value_str))   # <class 'str'>
```
</details>

---

## 7. Further Reading

- [Python Official Documentation: Data Types](https://docs.python.org/3/library/stdtypes.html)
- [PEP 8: Naming Conventions](https://peps.python.org/pep-0008/#naming-conventions)

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