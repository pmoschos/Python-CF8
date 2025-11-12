# 🧮 Python Floating-Point and Scientific Notation

This lesson explores how Python represents and manipulates floating-point numbers, including the use of scientific notation. You’ll learn about floating-point arithmetic, precision, and best practices for working with real numbers in Python.

---

## 1. Learning Objectives

- Understand how floating-point numbers are represented and used in Python.
- Use scientific notation to express very large or small numbers in Python.
- Perform arithmetic operations with floating-point numbers and interpret results.
- Recognize and explain common issues with floating-point precision.
- Apply best practices for comparing floating-point values.

---

## 2. Prerequisites

- Basic Python syntax (variables, assignment, print statements).
- Understanding of integers and arithmetic operations.
- Familiarity with the concept of data types.

---

## 3. Key Concepts

- **Float**: A data type representing real numbers with decimal points (e.g., `3.14`).
- **Scientific Notation**: A compact way to represent very large or small numbers, using `e` or `E` (e.g., `1.23e4` means `1.23 × 10⁴`).
- **Floating-Point Arithmetic**: Mathematical operations involving float values, subject to rounding errors.
- **Precision**: The accuracy with which a number is represented; floats have limited precision.
- **Rounding Error**: Small inaccuracies that occur because some decimal fractions cannot be represented exactly in binary.
- **Comparison Pitfall**: Directly comparing floats for equality can yield unexpected results due to precision issues.

---

## 4. Lecture Outline

### 0:00–0:05 — Introduction to Floating-Point Numbers
- What is a float? How does it differ from an integer?
- Examples: `x = 3.14`, `y = 2.0`

### 0:05–0:12 — Scientific Notation in Python
- Why use scientific notation?
- Syntax: `a = 1.5e3` (means 1500.0)
- Examples: Small and large numbers

### 0:12–0:18 — Arithmetic with Floats
- Addition, subtraction, multiplication, division
- Mixing ints and floats: `2 + 3.0` → `5.0`
- Example calculations

### 0:18–0:23 — Precision and Rounding Errors
- Demonstrate rounding errors: `0.1 + 0.2`
- Why do these errors occur?
- Implications for equality checks

### 0:23–0:27 — Best Practices for Comparing Floats
- Avoid `==` for floats; use a tolerance
- Example with `abs(a - b) < 1e-9`

### 0:27–0:30 — Q&A and Recap
- Review key takeaways
- Address student questions

---

## 5. Code Demos

```python
# Basic float assignment
PI = 3.1415926535
b = 2.0

# Print the value of PI and its type
print("Value of PI:", PI)
print("Type of PI:", type(PI))

print(b)  # Output: 2.0

# Scientific notation
x = 1.5e3   # 1.5 × 10^3 = 1500.0
y = 2.5e-4  # 2.5 × 10^-4 = 0.00025
print(x, y)  # Output: 1500.0 0.00025

# Arithmetic with floats
print(2 + 3.0)      # Output: 5.0
print(0.1 + 0.2)    # Output: 0.30000000000000004

# Comparing floats (bad vs. good)
print(0.1 + 0.2 == 0.3)  # Output: False (due to rounding error)
print(abs((0.1 + 0.2) - 0.3) < 1e-9)  # Output: True
```

---

## 6. Exercises

### 1. (Level 1, MCQ)
Which of the following is **not** a valid way to write a floating-point number in Python?
- a) `3.14`
- b) `2e5`
- c) `1.0e-3`
- d) `5,000.0`

<details>
<summary>Solution</summary>

**Answer:** d) `5,000.0`  
*Explanation: Commas are not allowed in numeric literals in Python.*
</details>

---

### 2. (Level 1, Short Answer)
What is the value of `a` after the following code runs?

```python
a = 4.2e2
```

<details>
<summary>Solution</summary>

**Answer:** `420.0`  
*Because `4.2e2` means `4.2 × 10² = 420.0`.*
</details>

---

### 3. (Level 2, Coding)
Write Python code to print the result of `0.1 + 0.2` and explain why it may not be exactly `0.3`.

<details>
<summary>Solution</summary>

```python
print(0.1 + 0.2)  # Output: 0.30000000000000004

# Explanation:
# Some decimal fractions cannot be represented exactly in binary floating-point,
# so the result is slightly off from 0.3.
```
</details>

---

### 4. (Level 2, Coding)
Given `a = 1.23e5` and `b = 123000.0`, write code to check if they are "close enough" to be considered equal, using a tolerance of `1e-6`.

<details>
<summary>Solution</summary>

```python
a = 1.23e5
b = 123000.0
print(abs(a - b) < 1e-6)  # Output: True
```
</details>

---

### 5. (Level 3, Coding)
Write a function `is_close(x, y, tol=1e-8)` that returns `True` if `x` and `y` are within `tol` of each other, and `False` otherwise. Use it to check if `0.1 + 0.2` is close to `0.3`.

<details>
<summary>Solution</summary>

```python
def is_close(x, y, tol=1e-8):
    return abs(x - y) < tol

print(is_close(0.1 + 0.2, 0.3))  # Output: True
```
</details>

---

## 8. Further Reading

- [Python 3 Documentation: Floating Point Arithmetic: Issues and Limitations](https://docs.python.org/3/tutorial/floatingpoint.html)

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