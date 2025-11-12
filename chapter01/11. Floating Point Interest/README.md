# 💸 Python Interest Calculation 📈

This lesson explores how to calculate interest using floating-point arithmetic in Python. You'll learn to write programs that compute the growth of an investment over time, understand the impact of floating-point precision, and apply these concepts to real-world financial scenarios.

---

## 1. Learning Objectives

- Understand how to represent and manipulate floating-point numbers in Python.
- Calculate simple and compound interest using Python code.
- Recognize the impact of floating-point precision in financial calculations.
- Write Python programs to model investment growth over multiple years.
- Debug and interpret floating-point calculation results.

---

## 2. Prerequisites

- Basic Python syntax (variables, arithmetic operators, input/output).
- Understanding of data types (integers, floats).
- Familiarity with loops and basic functions.
- Basic knowledge of mathematical operations (exponents, order of operations).

---

## 3. Key Concepts

- **Floating-Point Number**: A number with a decimal point, used to represent real numbers in Python (e.g., `3.14`).
- **Simple Interest**: Interest calculated only on the original principal.
- **Compound Interest**: Interest calculated on the principal and also on the accumulated interest.
- **Principal**: The initial amount of money invested or loaned.
- **Interest Rate**: The percentage at which interest is calculated, typically per year.
- **Precision Error**: Small inaccuracies that can occur when representing decimal numbers in binary floating-point.

---

## 4. Lecture Outline

### 0:00–0:05 — Introduction to Interest Calculations
- What is interest? Simple vs. compound interest.
- Why use floating-point numbers in financial calculations?
- Example: "If you invest $100 at 5% interest..."

### 0:05–0:15 — Floating-Point Numbers in Python
- Declaring floats: `balance = 100.0`
- Arithmetic with floats: addition, multiplication, exponentiation.
- Example: `balance * 1.05` to apply 5% interest.

### 0:15–0:25 — Calculating Compound Interest
- Formula: `final_amount = principal * (1 + rate) ** years`
- Step-by-step calculation for 3 years at 5% interest.
- Example: Show calculation by hand and in Python.

### 0:25–0:30 — Floating-Point Precision Issues
- Demonstrate small errors: `0.1 + 0.2 != 0.3`
- Why does this happen? (Brief explanation)
- Importance in financial applications.

### 0:30–0:35 — Coding a Year-by-Year Interest Table
- Use a loop to print balance for each year.
- Example: Table of balances for 10 years.

### 0:35–0:40 — Q&A and Summary
- Recap: floating-point, interest formulas, Python implementation.

---

## 5. Code Demos

```python
# Simple interest calculation (not compounded)
principal = 1000.0  # initial amount in dollars
rate = 0.05         # 5% interest per year
years = 3

# Simple interest: only on principal
simple_interest = principal * rate * years
print("Simple interest after 3 years:", simple_interest)
print("Total amount:", principal + simple_interest)
```

```python
# Compound interest calculation
principal = 1000.0
rate = 0.05
years = 3

# Compound interest: interest on interest
final_amount = principal * (1 + rate) ** years
print("Compound interest total after 3 years:", final_amount)
```

```python
# Demonstrating floating-point precision issue
a = 0.1 + 0.2
print("0.1 + 0.2 =", a)
print("Is 0.1 + 0.2 == 0.3?", a == 0.3)
```

---

## 6. Exercises

### 1. (Level 1, MCQ)
What is the result of the following code?

```python
balance = 200.0
rate = 0.1
years = 2
final = balance * (1 + rate) ** years
print(round(final, 2))
```

a) 220.0  
b) 240.0  
c) 242.0  
d) 242.00  

<details>
<summary>Solution</summary>

**Answer:** d) 242.00  
Calculation: 200 * (1.1)^2 = 200 * 1.21 = 242.00
</details>

---

### 2. (Level 1, Short Answer)
Write the Python expression to calculate the amount after 4 years if you invest $500 at 3% annual interest, compounded yearly.

<details>
<summary>Solution</summary>

```python
amount = 500 * (1 + 0.03) ** 4
```
</details>

---

### 3. (Level 2, MCQ)
Why might the following code print `False`?

```python
print(0.1 + 0.2 == 0.3)
```

a) Python does not support addition of floats  
b) Floating-point numbers can have small rounding errors  
c) `0.1 + 0.2` is exactly `0.3` in Python  
d) The `==` operator does not work for floats  

<details>
<summary>Solution</summary>

**Answer:** b) Floating-point numbers can have small rounding errors
</details>

---

## 7. Further Reading

- [Python Documentation: Floating Point Arithmetic](https://docs.python.org/3/tutorial/floatingpoint.html)
- [Investopedia: Compound Interest](https://www.investopedia.com/terms/c/compoundinterest.asp)

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