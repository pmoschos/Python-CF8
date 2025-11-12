# 🟢 Python Boolean Operations

This lesson introduces Boolean values and expressions in Python, focusing on their use in logical operations, comparisons, and control flow. You'll learn how to construct and evaluate Boolean expressions, use logical operators, and apply these concepts to practical programming problems.

---

## 1. Learning Objectives

- Understand what Boolean values are and how they are represented in Python.
- Construct and evaluate Boolean expressions using comparison and logical operators.
- Apply Boolean logic to control program flow with `if` statements.
- Recognize the difference between assignment (`=`) and equality (`==`) operators.
- Predict and explain the outcome of complex Boolean expressions.

---

## 2. Prerequisites

- Basic Python syntax (variables, numbers, strings).
- Familiarity with arithmetic operators (`+`, `-`, `*`, `/`).
- Understanding of simple `if` statements.

---

## 3. Key Concepts

- **Boolean Value**: A value that is either `True` or `False`.
- **Boolean Expression**: An expression that evaluates to a Boolean value.
- **Comparison Operator**: Operators that compare values (`==`, `!=`, `<`, `>`, `<=`, `>=`).
- **Logical Operator**: Operators that combine Boolean expressions (`and`, `or`, `not`).
- **Truth Table**: A table showing all possible values of logical expressions.
- **Assignment vs Equality**: `=` assigns a value; `==` checks if values are equal.

---

## 4. Lecture Outline

### 0:00–0:03 — Introduction to Boolean Values
- What are Boolean values? (`True`, `False`)
- Python's `bool` type.

### 0:03–0:10 — Boolean Expressions and Comparison Operators
- Creating Boolean expressions: `5 > 3`, `x == 10`
- Common comparison operators: `==`, `!=`, `<`, `>`, `<=`, `>=`
- Example: `a = 7; print(a != 5)`

### 0:10–0:18 — Logical Operators: `and`, `or`, `not`
- Combining expressions: `x > 5 and x < 10`
- Truth tables for `and`, `or`, `not`
- Example: `not (3 > 1)`

### 0:18–0:23 — Boolean Expressions in Control Flow
- Using Boolean expressions in `if` statements
- Example: `if age >= 18: print("Adult")`
- Short-circuit evaluation

### 0:23–0:28 — Common Pitfalls and Best Practices
- Assignment (`=`) vs Equality (`==`)
- Parentheses for clarity in complex expressions
- Example: `if (x > 0) and (y > 0): ...`

### 0:28–0:30 — Q&A and Summary
- Recap key points
- Address student questions

---

## 5. Code Demos

```python
# Define Boolean variables
a = True
b = False

# Print the type and value of each Boolean variable
print(type(a), a)
print(type(b), b)

# Demonstrate the logical OR operation
# The OR operation short-circuits; it stops evaluating once the truth value is determined.
# Since `a` is True, `b` is not evaluated in this case.
result = a or b  # `b` is not evaluated because `a` is `True`
print(result)  # Output: True

# Show how Booleans behave in arithmetic contexts
# Booleans in Python are a subclass of integers. True is 1, and False is 0.
print("True + True = ", True + True)  # Output will be 2, demonstrating arithmetic addition of Booleans


# Extra:
# Boolean values
print(True)   # Output: True
print(False)  # Output: False

# Comparison operators
x = 10
print(x == 10)    # Output: True
print(x != 5)     # Output: True
print(x > 7)      # Output: True
print(x <= 10)    # Output: True

# Logical operators
a = 5
b = 8
print(a > 0 and b < 10)  # Output: True
print(a < 0 or b < 10)   # Output: True
print(not (a == 5))      # Output: False

# Boolean expressions in control flow
age = 17
if age >= 18:
    print("Adult")
else:
    print("Minor")   # Output: Minor

# Assignment vs Equality
y = 3      # Assignment
print(y == 3)  # Equality check, Output: True
```

---

## 6. Exercises

### 1. (Level 1, MCQ)
Which of the following expressions evaluates to `False` in Python?

a) `5 == 5`  
b) `3 != 4`  
c) `7 < 2`  
d) `10 >= 10`

<details>
<summary>Solution</summary>

**Answer:** c) `7 < 2`
</details>

---

### 2. (Level 1, Short Answer)
What is the output of the following code?

```python
x = 4
print(x > 2 and x < 4)
```

<details>
<summary>Solution</summary>

**Output:** `False`
</details>

---

### 3. (Level 2, Coding)
Write a Python expression that checks if a variable `n` is **not** between 1 and 10 (inclusive).

<details>
<summary>Solution</summary>

```python
# n is not between 1 and 10 (inclusive)
not (1 <= n <= 10)
# or equivalently:
n < 1 or n > 10
```
</details>

---

### 4. (Level 2, Coding)
Given `a = 3`, `b = 7`, and `c = 5`, write a Python statement that prints `True` if **at least one** of the variables is greater than 6.

<details>
<summary>Solution</summary>

```python
a = 3
b = 7
c = 5
print(a > 6 or b > 6 or c > 6)  # Output: True
```
</details>

---


## 7. Auto-Grading Rubrics

**Exercise 1 (1 pt):**
- Correct option selected: 1 pt

**Exercise 2 (1 pt):**
- Correct Boolean output: 1 pt

**Exercise 3 (2 pts):**
- Correct use of logical/comparison operators: 1 pt
- Correct logic for "not between 1 and 10": 1 pt

**Exercise 4 (2 pts):**
- Correct use of `or` operator: 1 pt
- Correct comparison with 6: 1 pt

**Exercise 5 (4 pts):**
- Function defined with correct signature: 1 pt
- Checks length >= 8: 1 pt
- Checks substring `"123"`: 1 pt
- Returns correct Boolean value: 1 pt

---

## 8. Further Reading

- [Python Official Documentation: Boolean Operations](https://docs.python.org/3/library/stdtypes.html#boolean-values)
- [Python Comparison Operators](https://docs.python.org/3/reference/expressions.html#comparisons)

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