# 🌀 Set Operations in Python 🔀

This script demonstrates various set operations in Python, including intersection, union, difference, and symmetric difference. These operations are useful for comparing and manipulating sets of data.

## 1. Learning Objectives

- Understand the concept and properties of sets in Python.
- Perform fundamental set operations: union, intersection, difference, and symmetric difference.
- Apply set methods to solve practical programming problems.
- Distinguish between set operations and their corresponding operators/methods.
- Recognize use-cases where set operations are beneficial.

---

## 2. Prerequisites

- Basic Python syntax (variables, data types, functions).
- Familiarity with lists and tuples.
- Understanding of loops and basic control flow.

---

## 3. Key Concepts

- **Set**: An unordered collection of unique, immutable elements.
- **Union (`|` or `.union()`)**: Combines all unique elements from two sets.
- **Intersection (`&` or `.intersection()`)**: Elements common to both sets.
- **Difference (`-` or `.difference()`)**: Elements in one set but not the other.
- **Symmetric Difference (`^` or `.symmetric_difference()`)**: Elements in either set, but not both.
- **Subset/Superset**: A set is a subset if all its elements are in another set; superset is the reverse.
- **Set Methods**: Functions like `add()`, `remove()`, `update()`, etc., to manipulate sets.

---

## 4. Lecture Outline

### 0:00–0:05 — Introduction to Sets
- What is a set? How is it different from lists/tuples?
- Syntax: `{}` or `set()`
- Example: `a = {1, 2, 3}`

### 0:05–0:15 — Basic Set Operations
- Union: `a | b` or `a.union(b)`
- Intersection: `a & b` or `a.intersection(b)`
- Difference: `a - b` or `a.difference(b)`
- Symmetric Difference: `a ^ b` or `a.symmetric_difference(b)`
- Example walkthroughs

### 0:15–0:20 — Set Methods and Properties
- Adding/removing elements: `add()`, `remove()`, `discard()`
- Checking membership: `in`
- Subset/superset: `issubset()`, `issuperset()`

### 0:20–0:25 — Practical Applications
- Removing duplicates from lists
- Finding common or unique elements between datasets
- Example: Students enrolled in multiple courses

### 0:25–0:30 — Q&A and Summary
- Recap key operations and when to use them

---

## 5. Code Demos

```python
# Creating sets
a = {1, 2, 3}
b = {3, 4, 5}

# Union
print(a | b)  # Output: {1, 2, 3, 4, 5}

# Intersection
print(a & b)  # Output: {3}

# Difference
print(a - b)  # Output: {1, 2}

# Symmetric Difference
print(a ^ b)  # Output: {1, 2, 4, 5}

# Adding and removing elements
a.add(6)
print(a)      # Output: {1, 2, 3, 6}
a.remove(1)
print(a)      # Output: {2, 3, 6}
```

---

## 6. Exercises

### 1. (Level 1, MCQ)
Which of the following statements about Python sets is **false**?
- a) Sets can contain duplicate elements.
- b) Sets are unordered collections.
- c) Sets support mathematical set operations.
- d) Sets can be created using curly braces `{}`.

<details>
<summary>Solution</summary>

**Answer:** a) Sets can contain duplicate elements.
</details>

---

### 2. (Level 1, Short Answer)
What is the result of the following code?

```python
a = {1, 2, 3}
b = {2, 3, 4}
print(a & b)
```

<details>
<summary>Solution</summary>

**Output:** `{2, 3}`
</details>

---

### 3. (Level 2, Coding)
Write a Python statement to find all elements that are in either set `a` or set `b`, but not in both.

```python
a = {1, 2, 3}
b = {3, 4, 5}
# Your code here
```

<details>
<summary>Solution</summary>

```python
print(a ^ b)  # Output: {1, 2, 4, 5}
```
</details>

---

### 4. (Level 2, Coding)
Given two lists, remove duplicates and print the common elements.

```python
list1 = [1, 2, 2, 3, 4]
list2 = [3, 4, 4, 5, 6]
# Your code here
```

<details>
<summary>Solution</summary>

```python
set1 = set(list1)
set2 = set(list2)
print(set1 & set2)  # Output: {3, 4}
```
</details>

---

### 5. (Level 3, Coding)
Given three sets:

```python
a = {1, 2, 3, 4}
b = {3, 4, 5, 6}
c = {4, 5, 6, 7}
```

Write Python code to print all elements that are present in **exactly two** of the three sets.

<details>
<summary>Solution</summary>

```python
# Elements in exactly two sets:
result = ((a & b) | (b & c) | (a & c)) - (a & b & c)
print(result)  # Output: {3, 5, 6}
```
</details>

---

## Script Overview 📘

The script defines two sets and performs several operations to find common elements, all elements, elements in one set but not the other, and elements in either set but not both.

### :computer: Script Code

```python
def main():
    """
    Demonstrates set operations.
    """
    # Define two sets of products available in two different stores
    store_a_products = {"Apples", "Bananas", "Cherries", "Dates", "Watermelons"}
    store_b_products = {"Bananas", "Cherries", "Figs", "Grapes", "Melons"}

    # Find common products (intersection) available in both stores
    common_products = store_a_products & store_b_products
    print("Products available in both Store A and Store B:", common_products)
    # Alternatively, using the intersection method
    common_products = store_a_products.intersection(store_b_products)
    print("Products available in both Store A and Store B:", common_products)

    # Find all unique products (union) across both stores
    all_products = store_a_products | store_b_products
    print("All unique products across Store A and Store B:", all_products)
    # Alternatively, using the union method
    all_products = store_a_products.union(store_b_products)
    print("All unique products across Store A and Store B:", all_products)

    # Find products available in Store A but not in Store B (difference)
    store_a_exclusive = store_a_products - store_b_products
    print("Products available only in Store A:", store_a_exclusive)
    # Alternatively, using the difference method
    store_a_exclusive = store_a_products.difference(store_b_products)
    print("Products available only in Store A:", store_a_exclusive)

    # Find products available in Store B but not in Store A (difference)
    store_b_exclusive = store_b_products - store_a_products
    print("Products available only in Store B:", store_b_exclusive)
    # Alternatively, using the difference method
    store_b_exclusive = store_b_products.difference(store_a_products)
    print("Products available only in Store B:", store_b_exclusive)

    # Find products that are in either Store A or Store B but not in both (symmetric difference)
    unique_to_either_store = store_a_products ^ store_b_products
    print("Products available in either Store A or Store B but not both:", unique_to_either_store)
    # Alternatively, using the symmetric_difference method
    unique_to_either_store = store_a_products.symmetric_difference(store_b_products)
    print("Products available in either Store A or Store B but not both:", unique_to_either_store)

if __name__ == "__main__":
    main()
```

## Key Features 🌟
- **Set Operations**: Learn how to perform various set operations such as intersection, union, difference, and symmetric difference.
- **Methods**: Understand the use of set methods like `intersection`, `union`, `difference`, and `symmetric_difference`.

## Technical Requirements 🔧
- **Python Version**: Python 3.x recommended
- **External Libraries**: None, only the built-in set operations

## Installation and Setup 🚀
No installation is required, as the script can be run directly from any Python-enabled environment:

1. Ensure Python 3.x is installed on your machine.
2. Save the script as `20_set_operations.py`.
3. Open a terminal or command prompt.
4. Navigate to the directory containing `20_set_operations.py`.
5. Run the script with: `python 20_set_operations.py`.

## Usage Example 📋
Execute the script to see how set operations are performed. The script will output the common elements, all elements, elements in one set but not the other, and elements in either set but not both.

📢 Stay Updated
Be sure to ⭐ this repository to keep up with updates and new learning materials!

## 📄 License
🔐 This project is protected under the MIT License.

## Contact 📧
Panagiotis Moschos - pan.moschos86@gmail.com

🔗 Note: This is a Python script and requires a Python interpreter to run.

<h1 align="center">Happy Coding 👨‍💻</h1>
<p align="center">
  Made with ❤️ by Panagiotis Moschos (https://github.com/pmoschos)
</p>
