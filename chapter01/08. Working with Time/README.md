# 🕒 Python Time Conversion

The script prompts the user to enter a total number of seconds and then calculates how many days, hours, minutes, and seconds that amount of time corresponds to. This showcases how to perform integer division and modulus operations to break down time into more understandable units.

Extra info: Also, this lesson introduces Python's tools for working with time, focusing on converting between different time representations. You'll learn to use the `time` module to retrieve the current time, convert between timestamps and human-readable formats, and format time strings for display or processing.

---

## 1. Learning Objectives

- Understand the difference between Unix timestamps and human-readable time formats.
- Use Python's `time` module to get the current time in various formats.
- Convert between timestamps and formatted time strings.
- Format and parse time strings using `strftime` and `strptime`.
- Apply time conversion techniques to real-world programming tasks.

---

## 2. Prerequisites

- Basic Python syntax (variables, functions, imports).
- Familiarity with strings and string formatting.
- Understanding of basic data types (integers, floats, strings).

---

## 3. Key Concepts

- **Unix Timestamp**: The number of seconds since January 1, 1970 (the Unix epoch).
- **`time.time()`**: Returns the current time as a Unix timestamp (float).
- **`time.localtime()`**: Converts a timestamp to a struct_time in local time.
- **`time.gmtime()`**: Converts a timestamp to a struct_time in UTC.
- **`time.strftime(fmt, t)`**: Formats a struct_time as a string according to a format string.
- **`time.strptime(s, fmt)`**: Parses a string into a struct_time according to a format string.
- **`struct_time`**: A named tuple representing a time (year, month, day, hour, minute, second, etc.).

---

## 4. Lecture Outline

### 0:00–0:05 — Introduction to Time in Programming
- Why do we need to work with time?
- Unix timestamp vs. human-readable formats.

### 0:05–0:15 — Getting the Current Time
- Using `time.time()` to get the current timestamp.
- Example: `print(time.time())`
- Converting timestamp to local time with `time.localtime()`.
- Example: `print(time.localtime())`

### 0:15–0:20 — Formatting and Parsing Time Strings
- Using `time.strftime()` to create custom time strings.
- Example: Formatting as "YYYY-MM-DD HH:MM:SS".
- Parsing a string back to a struct_time with `time.strptime()`.

### 0:20–0:25 — Time Conversion in Practice
- Converting between timestamps and formatted strings.
- Example: Displaying the current time in a user-friendly format.
- Parsing user input into timestamps.

### 0:25–0:30 — Q&A and Summary
- Recap key functions: `time.time()`, `time.localtime()`, `time.strftime()`, `time.strptime()`.
- Common pitfalls (e.g., time zones, format mismatches).

---

## 5. Code Demos

```python
# Constants for converting units of time
SECONDS_IN_A_MINUTE = 60
SECONDS_IN_AN_HOUR = 3600
SECONDS_IN_A_DAY = 86400

# Prompt the user to enter the total number of seconds
total_seconds = int(input("Enter the number of seconds: "))
# Example conversion: 105310 seconds is equal to: 1 day, 5 hours, 15 minutes, 10 seconds

# Calculate the number of days from the total seconds and the remainder
days = total_seconds // SECONDS_IN_A_DAY
seconds_remaining = total_seconds % SECONDS_IN_A_DAY

# Calculate the number of hours from the remaining seconds
hours = seconds_remaining // SECONDS_IN_AN_HOUR
seconds_remaining %= SECONDS_IN_AN_HOUR  # Update the seconds_remaining by applying modulus

# Calculate the number of minutes from the updated remaining seconds
minutes = seconds_remaining // SECONDS_IN_A_MINUTE
seconds_remaining %= SECONDS_IN_A_MINUTE  # Further reduce the remaining seconds

# The final value of seconds_remaining is the number of seconds
seconds = seconds_remaining

# Display the results in a clear, formatted way
print(f"{total_seconds} seconds is equal to:")
print(f"{days} days, {hours} hours, {minutes} minutes, {seconds} seconds")

# Extra info:
# Working with time module (We will also check it later on with extended examples)
import time

# Get the current Unix timestamp
timestamp = time.time()
print("Current timestamp:", timestamp)

# Convert timestamp to local time (struct_time)
local_time = time.localtime(timestamp)
print("Local time struct:", local_time)

# Format local time as a readable string
formatted_time = time.strftime("%Y-%m-%d %H:%M:%S", local_time)
print("Formatted local time:", formatted_time)

# Parse a time string back into struct_time
time_string = "2024-06-01 15:30:00"
parsed_time = time.strptime(time_string, "%Y-%m-%d %H:%M:%S")
print("Parsed struct_time:", parsed_time)

# Convert struct_time to timestamp
timestamp_from_struct = time.mktime(parsed_time)
print("Timestamp from struct_time:", timestamp_from_struct)
```

---

## 6. Exercises

### 1. (Level 1, MCQ)
Which function returns the current time as a Unix timestamp (seconds since epoch)?
- a) `time.strftime()`
- b) `time.time()`
- c) `time.localtime()`
- d) `time.strptime()`

<details>
<summary>Solution</summary>

**Answer:** b) `time.time()`
</details>

---

### 2. (Level 1, Short Answer)
What is the output type of `time.localtime()`?

<details>
<summary>Solution</summary>

**Answer:** `struct_time` (a named tuple representing time components)
</details>

---

### 3. (Level 2, Coding)
Write Python code to print the current date and time in the format `YYYY-MM-DD HH:MM:SS`.

<details>
<summary>Solution</summary>

```python
import time
print(time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()))
```
</details>

---

### 4. (Level 2, Coding)
Given the string `"2024-06-01 12:00:00"`, write code to convert it to a Unix timestamp.

<details>
<summary>Solution</summary>

```python
import time
s = "2024-06-01 12:00:00"
t = time.strptime(s, "%Y-%m-%d %H:%M:%S")
timestamp = time.mktime(t)
print(timestamp)
```
</details>

---

## 7. Further Reading

- [Python Docs: time module](https://docs.python.org/3/library/time.html)

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