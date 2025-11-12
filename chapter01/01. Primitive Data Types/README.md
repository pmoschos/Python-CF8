# 🟦 Basic Python Variable and Print Example 2

This lesson explores how to declare variables of different primitive data types in Python and display their values using the `print()` function. We'll focus on practical examples and best practices for advanced beginners and intermediate learners.

---

## 1. Learning Objectives

- Understand how to declare and assign values to variables of different primitive data types in Python.
- Use the `print()` function to display variable values and formatted output.
- Recognize Python's dynamic typing and how it affects variable assignment.
- Apply best practices for naming and using variables.
- Identify and correct common mistakes when working with variables and printing in Python.

---

## 2. Prerequisites

- Basic familiarity with Python syntax (indentation, statements).
- Understanding of what a variable is in programming.
- Ability to run Python scripts in an interpreter or IDE.

---

## 3. Key Concepts

- **Variable**: A named location in memory to store data.
- **Primitive Data Type**: Basic types like `int`, `float`, `str`, and `bool`.
- **Assignment (`=`)**: The operator used to assign a value to a variable.
- **Dynamic Typing**: Python variables can change type based on the assigned value.
- **`print()` Function**: Used to output data to the console.
- **String Concatenation**: Combining strings using `+` or formatted strings.

---

## 4. Lecture Outline

### 0:00–0:05 — Introduction to Variables and Data Types
- What is a variable?
- Primitive data types in Python: `int`, `float`, `str`, `bool`
- Example: Assigning values to variables

### 0:05–0:10 — Variable Assignment and Dynamic Typing
- Assigning different types to variables
- Reassigning variables to new types
- Example: `x = 5`, then `x = "hello"`

### 0:10–0:15 — Using the `print()` Function
- Basic usage: `print(variable)`
- Printing multiple variables: `print(a, b, c)`
- Concatenating strings and variables
- Example: `print("Age:", age)`

### 0:15–0:20 — Formatting Output
- Using commas vs. `+` for concatenation
- f-strings for readable output: `print(f"Name: {name}, Age: {age}")`
- Example: Displaying all variable values in a single line

### 0:20–0:25 — Best Practices and Common Errors
- Good variable names
- Avoiding type errors (e.g., concatenating string and int)
- Q&A and summary

---

## 5. Code Demos

```python
# Example 1: Declaring variables of different types
name = "Alice"        # str
age = 30              # int
height = 1.65         # float
is_student = True     # bool

# Example 2: Printing variables individually
print(name)
print(age)
print(height)
print(is_student)

# Example 3: Printing with descriptive text
print("Name:", name)
print("Age:", age)
print("Height:", height, "meters")
print("Student status:", is_student)

# Example 4: Using f-strings for formatted output (Python 3.6+)
print(f"{name} is {age} years old and {height} meters tall. Student: {is_student}")

# Example 5: Demonstrating dynamic typing
x = 42
print("x is now:", x)
x = "forty-two"
print("x is now:", x)
```

---

## 6. Exercises

### 1. (Level 1, MCQ)
Which of the following is a valid variable assignment in Python?
- a) `int age = 25`
- b) `age := 25`
- c) `age = 25`
- d) `25 = age`

<details>
<summary>Solution</summary>

**Answer:** c) `age = 25`
</details>

---

### 2. (Level 1, Short Answer)
What will be the output of the following code?

```python
name = "Bob"
print("Hello", name)
```

<details>
<summary>Solution</summary>

**Output:** `Hello Bob`
</details>

---

### 3. (Level 2, Coding)
Write Python code to declare a variable `temperature` with the value `22.5` (float), and print:  
`The temperature is 22.5 degrees.`

<details>
<summary>Solution</summary>

```python
temperature = 22.5
print("The temperature is", temperature, "degrees.")
```
</details>

---

### 4. (Level 2, Coding)
Given the following variables:

```python
first_name = "Jane"
last_name = "Doe"
age = 28
```

Print the sentence:  
`Jane Doe is 28 years old.`  
using an f-string.

<details>
<summary>Solution</summary>

```python
print(f"{first_name} {last_name} is {age} years old.")
```
</details>

---

### 5. (Level 3, Coding)
Write a Python script that:
- Declares variables for a person's name (string), age (int), height (float), and student status (bool).
- Prints all the information in a single, well-formatted sentence using an f-string.

Example output:  
`Name: Alex, Age: 21, Height: 1.75m, Student: True`

<details>
<summary>Solution</summary>

```python
name = "Alex"
age = 21
height = 1.75
is_student = True

print(f"Name: {name}, Age: {age}, Height: {height}m, Student: {is_student}")
```
</details>

---

## 7. Further Reading

- [Python Official Documentation: Built-in Types](https://docs.python.org/3/library/stdtypes.html)
- [Python Official Documentation: print() function](https://docs.python.org/3/library/functions.html#print)

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