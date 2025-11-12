# 🧑‍💻 Python User Interaction and Data Conversion with IF-Else Statements

This lesson explores how to interact with users in Python using `input()`, convert user input to different data types, and make decisions with `if-else` statements. These are foundational skills for writing interactive and robust Python programs.

---

## 1. Learning Objectives

- Use `input()` to receive user input in Python.
- Convert user input from strings to integers or floats.
- Apply `if-else` statements to control program flow based on user input.
- Handle basic errors that may occur during data conversion.
- Write simple interactive programs that respond to user choices.

---

## 2. Prerequisites

- Basic Python syntax (variables, print statements).
- Understanding of data types: `str`, `int`, `float`.
- Familiarity with indentation and code blocks.

---

## 3. Key Concepts

- **input()**: Function to get user input as a string.
- **Type Conversion**: Changing data from one type to another, e.g., `int('5')` or `float('3.14')`.
- **if-else Statement**: Conditional logic to execute code based on whether a condition is true or false.
- **Indentation**: Python uses indentation to define code blocks.
- **Error Handling**: Anticipating and managing errors, especially when converting input.

---

## 4. Lecture Outline

### 0:00–0:05 — Introduction to User Input
- Why interact with users?
- The `input()` function always returns a string.
- Example: `name = input("Enter your name: ")`

### 0:05–0:10 — Data Conversion Basics
- User input is a string by default.
- Converting to integer: `age = int(input("Enter your age: "))`
- Converting to float: `height = float(input("Enter your height in meters: "))`
- Example: What happens if the user enters non-numeric input?

### 0:10–0:18 — Using IF-Else Statements
- Syntax of `if`, `else`, and `elif`.
- Making decisions based on user input.
- Example: Checking if a user is old enough to vote.

### 0:18–0:23 — Combining Input, Conversion, and IF-Else
- Building interactive scripts that respond to user data.
- Example: Grading system based on user’s score.

### 0:23–0:27 — Error Handling (Intro)
- What happens if conversion fails?
- Brief mention of `try-except` (optional for advanced beginners).

### 0:27–0:30 — Q&A and Summary
- Recap key takeaways.
- Common pitfalls (e.g., forgetting to convert input).

---

## 5. Code Demos

```python
# 1. Basic input and output
name = input("What is your name? ")
print("Hello,", name)

# 2. Input with type conversion
age = int(input("Enter your age: "))  # Converts string to integer
print("Next year, you will be", age + 1)

# 3. Using if-else with user input
score = float(input("Enter your test score (0-100): "))
if score >= 60:
    print("You passed!")
else:
    print("You failed.")

# 4.  Request a yes/no answer to determine if the user is a student, converting to lowercase and comparing to 'yes'
is_student = input("Are you a student? (yes/no): ").lower() == 'yes'

# Condition to check if the user is a student and print the corresponding status
if is_student:
    print("You are a student.")
else:
    print("You are not a student.")
    
# Print the user's age and height, formatting the height to two decimal places
print("Your age is {}, and your height is {:.2f} meters.".format(age, height))
```

---

## 6. Exercises

### 1. (Level 1, MCQ)
What is the type of the value returned by `input()` in Python?

a) int  
b) float  
c) str  
d) bool  

<details>
<summary>Solution</summary>

**Answer:** c) str
</details>

---

### 2. (Level 1, Short Answer)
What will be printed by the following code if the user enters `7`?

```python
x = input("Enter a number: ")
print(x * 2)
```

<details>
<summary>Solution</summary>

**Output:** `77` (since `x` is a string, so `"7" * 2` is `"77"`)
</details>

---

### 3. (Level 2, Coding)
Write a Python program that asks the user for their age and prints "Adult" if the age is 18 or older, otherwise prints "Minor".

<details>
<summary>Solution</summary>

```python
age = int(input("Enter your age: "))
if age >= 18:
    print("Adult")
else:
    print("Minor")
```
</details>

---

### 4. (Level 2, Coding)
Write a program that asks the user to enter a number. If the number is even, print "Even"; if it is odd, print "Odd".

<details>
<summary>Solution</summary>

```python
num = int(input("Enter a number: "))
if num % 2 == 0:
    print("Even")
else:
    print("Odd")
```
</details>

---

### 5. (Level 3, Coding)
Ask the user to enter a floating-point number. If the number is positive, print its square root (use `** 0.5`). If the number is negative, print "Cannot compute square root of a negative number".

<details>
<summary>Solution</summary>

```python
num = float(input("Enter a number: "))
if num >= 0:
    print("Square root is", num ** 0.5)
else:
    print("Cannot compute square root of a negative number")
```
</details>

---


## 7. Further Reading

- [Python Official Documentation: input()](https://docs.python.org/3/library/functions.html#input)
- [Python Official Documentation: if Statements](https://docs.python.org/3/tutorial/controlflow.html#if-statements)

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