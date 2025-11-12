# 🖱️ Python User Interaction and Data Conversion

This lesson explores how Python programs interact with users through input, and how to safely convert input data between types. You'll learn to build interactive scripts that handle user input robustly and perform essential data conversions.

---

## 1. Learning Objectives

- Use the `input()` function to receive user input in Python.
- Understand that input is always received as a string, and why conversion is necessary.
- Convert input strings to other data types (e.g., `int`, `float`) safely.
- Handle basic errors that arise from invalid input conversions.
- Write interactive scripts that process and respond to user input.

---

## 2. Prerequisites

- Basic Python syntax (variables, assignment, print statements).
- Familiarity with Python data types: `str`, `int`, `float`.
- Understanding of simple functions and expressions.

---

## 3. Key Concepts

- **`input()` Function**: Reads a line of text from the user as a string.
- **Type Conversion**: Changing data from one type to another (e.g., `str` to `int`).
- **`int()` / `float()`**: Functions to convert strings to integers or floating-point numbers.
- **Error Handling**: Managing situations where conversion fails (e.g., user enters non-numeric input).
- **Prompt**: The message displayed to the user when requesting input.

---

## 4. Lecture Outline

### 0:00–0:05 — Introduction: Why User Input?
- Programs often need to interact with users.
- Example: Calculators, games, data entry.

### 0:05–0:15 — The `input()` Function
- Syntax: `input("Prompt message")`
- Always returns a string.
- Example:
  ```python
  name = input("Enter your name: ")
  print("Hello,", name)
  ```

### 0:15–0:25 — Data Conversion Basics
- Problem: Numbers entered are strings, not numbers.
- Converting input:
  - `age = int(input("Enter your age: "))`
  - `height = float(input("Enter your height in meters: "))`
- Show what happens if conversion fails.

### 0:25–0:30 — Error Handling (Intro)
- What if the user enters invalid data?
- Brief mention of `try`/`except` for robust scripts.
- Example: Catching `ValueError`.

### 0:30–0:35 — Putting It Together: Interactive Example
- Build a small script that asks for two numbers and prints their sum.
- Discuss the flow: prompt → input (string) → convert → use.

---

## 5. Code Demos

```python
# 1. Basic input and output
name = input("What is your name? ")
print("Hello,", name)

# 2. Input is always a string
age_str = input("Enter your age: ")
print("You entered:", age_str, "which is of type", type(age_str))

# 3. Converting input to int
age = int(input("Enter your age: "))
print("Next year, you will be", age + 1)

# 4. Handling float input
height = float(input("Enter your height in meters: "))
print("Your height in centimeters is", height * 100)

# 5. Basic error handling (optional) - Exceptions will be covered in details in next chapter.
try:
    number = int(input("Enter an integer: "))
    print("You entered:", number)
except ValueError:
    print("That was not a valid integer!")
```

---

## 6. Exercises

### 1. (Level 1, MCQ)
What is the type of the value returned by `input()` in Python 3?

a) `int`  
b) `float`  
c) `str`  
d) Depends on the input

<details>
<summary>Solution</summary>

**Answer:** c) `str`
</details>

---

### 2. (Level 1, Short Answer)
What will be printed by the following code if the user enters `42`?

```python
num = input("Enter a number: ")
print(num + num)
```

<details>
<summary>Solution</summary>

**Output:**  
`4242` (because `input()` returns a string, so string concatenation occurs)
</details>

---

### 3. (Level 2, Coding)
Write a Python program that asks the user for their birth year and prints their age (assuming the current year is 2024).

<details>
<summary>Solution</summary>

```python
birth_year = int(input("Enter your birth year: "))
age = 2024 - birth_year
print("You are", age, "years old.")
```
</details>

---

### 4. (Level 2, Coding)
Ask the user for two numbers and print their product. Make sure to convert the input to the correct type.

<details>
<summary>Solution</summary>

```python
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))
product = num1 * num2
print("The product is:", product)
```
</details>

---

### 5. (Level 3, Coding)
Write a program that asks the user to enter an integer. If the user enters something that is not an integer, print `"Invalid input!"` instead of crashing.

<details>
<summary>Solution</summary>

```python
try:
    value = int(input("Enter an integer: "))
    print("You entered:", value)
except ValueError:
    print("Invalid input!")
```
</details>

---

## 7. Further Reading

- [Python Official Documentation: input()](https://docs.python.org/3/library/functions.html#input)
- [Python Official Documentation: Type Conversion](https://docs.python.org/3/library/functions.html#int)

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