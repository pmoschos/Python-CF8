# 🐍 Python Variables and Printing Options 🖨️

This lesson explores how to create and use variables in Python, and how to control output formatting using various print statement options. You'll learn to write readable, well-formatted Python programs.

---

## 1. Learning Objectives

- Understand how to declare and assign values to variables in Python.
- Recognize Python's variable naming rules and conventions.
- Use the `print()` function with different options to control output.
- Format output using separators (`sep`), end characters (`end`), and string concatenation.
- Apply variable and print concepts to write clear, informative Python scripts.

---

## 2. Prerequisites

- Basic understanding of Python syntax (indentation, statements).
- Familiarity with data types: `int`, `float`, `str`.
- Ability to run Python scripts in an interpreter or IDE.

---

## 3. Key Concepts

- **Variable**: A named reference to a value stored in memory.
- **Assignment (`=`)**: The operator used to assign a value to a variable.
- **Naming Rules**: Variable names must start with a letter or `_`, and can include letters, digits, and underscores.
- **`print()` Function**: Outputs text or variables to the console.
- **Separator (`sep`)**: An optional argument in `print()` that specifies the string inserted between values (default is a space).
- **End Character (`end`)**: An optional argument in `print()` that specifies what is printed at the end (default is newline `\n`).
- **String Concatenation**: Combining strings using `+` or formatting methods.

---

## 4. Lecture Outline

### 0:00–0:05 — Introduction to Variables
- What is a variable? Why use variables?
- Syntax: `variable_name = value`
- Example: `name = "Alice"`

### 0:05–0:12 — Variable Naming Rules and Conventions
- Valid and invalid variable names
- Case sensitivity
- Good naming practices

### 0:12–0:20 — The `print()` Function Basics
- Printing literals and variables
- Multiple arguments in `print()`
- Example: `print("Hello", name)`

### 0:20–0:25 — Advanced Print Options
- Using `sep` to change separators
- Using `end` to change line endings
- String concatenation and formatting
- Example: `print("A", "B", sep="-", end="!")`

### 0:25–0:30 — Q&A and Summary
- Recap: variables, naming, print options
- Common mistakes and troubleshooting

---

## 5. Code Demos

```python
# Declaring and assigning variables
age = 25
name = "Alice"
height = 1.68  # in meters

# Printing variables
print("Name:", name)
print("Age:", age)
print("Height:", height, "meters")

# Printing multiple values with default separator (space)
print(name, age, height)

# Using 'sep' to change separator
print(name, age, height, sep=" | ")

# Using 'end' to change line ending
print("This is the first line.", end=" ")
print("This is on the same line.")

# String concatenation
print("Hello, " + name + "!")

# Mixing variables and strings
print(f"{name} is {age} years old and {height} meters tall.")
```

---

## 6. Exercises

### 1. (Level 1, MCQ)
Which of the following is a valid Python variable name?
- a) `2nd_place`
- b) `firstName`
- c) `user-name`
- d) `class`

<details>
<summary>Solution</summary>

**Answer:** b) `firstName`
- `2nd_place` starts with a digit (invalid)
- `user-name` contains a hyphen (invalid)
- `class` is a reserved keyword (invalid)
</details>

---

### 2. (Level 1, Short Answer)
What will be the output of the following code?

```python
a = 5
b = 10
print(a, b, sep="---")
```

<details>
<summary>Solution</summary>

**Output:**  
`5---10`
</details>

---

### 3. (Level 2, Coding)
Write Python code to declare a variable `city` with value `"Paris"` and print the message:  
`Welcome to Paris!`  
using string concatenation.

<details>
<summary>Solution</summary>

```python
city = "Paris"
print("Welcome to " + city + "!")
```
</details>

---

### 4. (Level 2, Coding)
Given the variables:

```python
first = "Ada"
last = "Lovelace"
```

Print the full name separated by a hyphen (`-`) and end the output with three exclamation marks (`!!!`) (no newline after).

<details>
<summary>Solution</summary>

```python
print(first, last, sep="-", end="!!!")
```
</details>

---

### 5. (Level 3, Coding)
Write a program that asks the user for their favorite color and animal (use `input()`), then prints:  
`Your favorite color is <color> and your favorite animal is <animal>.`  
All on one line, using only one `print()` statement and formatted string literals (f-strings).

<details>
<summary>Solution</summary>

```python
color = input("Enter your favorite color: ")
animal = input("Enter your favorite animal: ")
print(f"Your favorite color is {color} and your favorite animal is {animal}.")
```
</details>

---

## 7. Further Reading

- [Python Official Documentation: print()](https://docs.python.org/3/library/functions.html#print)
- [Python Official Documentation: Variables](https://docs.python.org/3/reference/simple_stmts.html#assignment-statements)

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