# ✨ Python Magic Methods - Integer Limitations

This lesson explores Python's magic methods (also known as dunder methods), which enable operator overloading and customization of object behavior. You'll learn how these special methods work, how to implement them, and how they relate to Python's data model.

---

## 1. Learning Objectives

- Understand what magic methods (dunder methods) are and why they exist in Python.
- Recognize the naming conventions and common use cases for magic methods.
- Implement basic magic methods to customize object behavior (e.g., `__add__`, `__sub__`).
- Explain how magic methods enable operator overloading and integration with Python's built-in functions.
- Identify the role of magic methods in customizing class behavior for arithmetic, comparison, and type conversion.

---

## 2. Prerequisites

- Basic Python class and object syntax.
- Understanding of functions and methods.
- Familiarity with Python's built-in data types (int, str, list, etc.).
- Experience with operators and built-in functions.

---

## 3. Key Concepts

- **Magic Method (Dunder Method)**: Special methods with double underscores before and after their names (e.g., `__add__`, `__str__`). Used to define how objects behave with built-in operations.

- **`__add__`**, **`__sub__`**, etc.: Define behavior for arithmetic operators.

---

## 4. Lecture Outline

### 0:00–0:05 — Introduction to Magic Methods
- What are magic methods? Why are they called "dunder" methods?
- Examples:  `__add__`.

---

## 5. Code Demos

```python
# Initialize two integer variables
a = 10
b = 20

# Perform addition and store the result in a variable
result = a + b
# Print the result of the addition
print("a + b =", result)

# Print a separator line for clarity in output
print("---------")

# Display the data type of variable 'a'
print("Type of a:", type(a))

# Using the magic method __add__() to perform the addition
# Magic methods in Python are special methods which add "magic" to your classes.
# __add__ is one of these magic methods that allows the object of the class to use the + operator.
magic_result = a.__add__(b)
# Print the result obtained using the magic method
print("a + b =", magic_result)
```

---

## 6. Exercises

### 1. (Level 1, MCQ)
Which of the following is **not** a magic method in Python?

a) `__init__`  
b) `__str__`  
c) `__add__`  
d) `init`  

<details>
<summary>Solution</summary>

**Answer:** d) `init`
</details>

---

### 2. (Level 1, Short Answer)
What is the purpose of the `__str__` magic method in a Python class?

<details>
<summary>Solution</summary>

**Answer:**  
The `__str__` method returns a human-readable string representation of the object, used by `print()` and `str()`.
</details>

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