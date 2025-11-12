# 🧮 Python Integer Range

This lesson introduces Python's integer range, focusing on how Python handles integer values, their limits, and related functions. You'll learn how Python's integer type differs from other languages, how to work with very large numbers, and how to use built-in functions to manipulate integers.

---

## 1. Learning Objectives

- Understand how Python represents and manages integer values.
- Identify the practical limits (if any) of integers in Python.
- Use built-in integer functions such as `int()`, `abs()`, `pow()`, and `divmod()`.
- Recognize the differences between Python's integer type and those in other programming languages.
- Apply integer functions to solve real-world programming problems.

---

## 2. Prerequisites

- Basic Python syntax (variables, expressions, functions).
- Familiarity with data types (especially numbers).
- Understanding of arithmetic operations.

---

## 3. Key Concepts

- **Integer (`int`)**: A whole number, positive or negative, without decimals, of unlimited size in Python 3.
- **Arbitrary Precision**: Python's `int` type can represent integers of any size, limited only by available memory.
- **`int()` Function**: Converts a value to an integer.
- **`abs()` Function**: Returns the absolute (non-negative) value of a number.
- **`pow()` Function**: Raises a number to a power; can also perform modular exponentiation.
- **`divmod()` Function**: Returns a tuple containing the quotient and remainder of a division.
- **Integer Overflow**: In Python 3, integers do not overflow; they grow as needed (unlike in many other languages).

---

## 4. Lecture Outline

### 0:00–0:05 — Introduction to Integers in Python
- What is an integer?
- How does Python's `int` differ from C/Java's `int`?
- Example: Assigning small and very large integers.

### 0:05–0:12 — Integer Limits and Arbitrary Precision
- Demonstrate that Python integers can be very large.
- Discuss memory limitations vs. fixed-size types in other languages.
- Example: Calculating `2**1000`.

### 0:12–0:20 — Built-in Integer Functions
- `int()`: Type conversion and base conversion.
    - Example: `int('101', 2)` → 5
- `abs()`: Getting absolute values.
    - Example: `abs(-42)` → 42
- `pow()`: Exponentiation and modular exponentiation.
    - Example: `pow(2, 10)` and `pow(2, 10, 1000)`
- `divmod()`: Simultaneously getting quotient and remainder.
    - Example: `divmod(17, 5)` → (3, 2)

### 0:20–0:25 — Practical Applications and Edge Cases
- When to use arbitrary-precision integers.
- Handling user input and type conversion.
- Example: Reading numbers as strings and converting to int.

### 0:25–0:30 — Q&A and Summary
- Recap: Python's integer flexibility and useful functions.
- Compare with integer handling in other languages.

---

## 5. Code Demos

```python
import sys

# Largest integer 
max_int = sys.maxsize
print("Max int:", max_int)

# Smallest integer 
min_int = -sys.maxsize - 1
print("Min int:", min_int)

# For a 64-bit system, you would get:
# Max size: 9223372036854775807
# Max int: 9223372036854775807
# Min int: -9223372036854775808

# For a 32-bit system, you would get:
# Max size: 2147483647
# Max int: 2147483647
# Min int: -2147483648

# Python integers can be arbitrarily large
x = 123456789012345678901234567890
print(x)  # Output: 123456789012345678901234567890


# Extra info

# Extra 1:
# int() function: converting string to integer, with base
binary_str = '1011'
print(int(binary_str, 2))  # Output: 11

# abs() function: absolute value
print(abs(-42))  # Output: 42

# Extra 2:
# pow() function: exponentiation and modular exponentiation
print(pow(2, 10))        # Output: 1024
print(pow(2, 10, 1000))  # Output: 24 (1024 % 1000)

# Extra 3:
# divmod() function: quotient and remainder
q, r = divmod(17, 5)
print(q, r)  # Output: 3 2
```

---

## 6. Exercises

### 1. (Level 1, MCQ)
Which statement about Python 3 integers is **true**?
- a) Python 3 integers have a fixed maximum value.
- b) Python 3 integers can grow as large as memory allows.
- c) Python 3 integers overflow at 2³¹-1.
- d) Python 3 does not support negative integers.

<details>
<summary>Solution</summary>

**Answer:** b) Python 3 integers can grow as large as memory allows.
</details>

---

### 2. (Level 1, Short Answer)
What is the output of the following code?

```python
print(int('110', 2))
```

<details>
<summary>Solution</summary>

**Output:** 6
</details>

---

### 3. (Level 2, Coding)
Write a Python statement that calculates the absolute value of the difference between -50 and 23.

<details>
<summary>Solution</summary>

```python
print(abs(-50 - 23))  # Output: 73
```
</details>

---

### 4. (Level 2, Coding)
Use `divmod()` to divide 123 by 7 and print both the quotient and remainder.

<details>
<summary>Solution</summary>

```python
q, r = divmod(123, 7)
print(q, r)  # Output: 17 4
```
</details>

---

### 5. (Level 3, Coding)
Write a function that takes a string representing a number in base 8 (octal), converts it to an integer, raises it to the 5th power, and returns the result modulo 1000.

```python
def octal_power_mod(s):
    # Your code here
```

Test with: `print(octal_power_mod('12'))`  # '12' in octal is 10 in decimal

<details>
<summary>Solution</summary>

```python
def octal_power_mod(s):
    n = int(s, 8)
    return pow(n, 5, 1000)

print(octal_power_mod('12'))  # Output: 0 (10**5 = 100000, 100000 % 1000 = 0)
```
</details>

---

## 7. Further Reading

- [Python 3 Documentation: Built-in Types — int](https://docs.python.org/3/library/functions.html#int)
- [Python 3 Documentation: Built-in Functions](https://docs.python.org/3/library/functions.html)
- [Python 3 Documentation: Numeric Types — int, float, complex](https://docs.python.org/3/library/stdtypes.html#numeric-types-int-float-complex)

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