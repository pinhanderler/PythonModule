# Python Conditional Statements

## Introduction

This guide aims to explain the basic conditional statements in Python for those who are new to Python programming. Conditional statements allow your program to follow different paths depending on certain conditions.

### Basic Conditional Statements

#### If Statement

The `if` statement allows certain code blocks to be executed when a specific condition is true.

```python
x = 10

if x > 5:
    print("x is greater than 5")
```

#### If-Else Statement

The `if-else` statement executes a certain code block when a condition is true; otherwise, it executes another code block.

```python
x = 3

if x > 5:
    print("x is greater than 5")
else:
    print("x is less than or equal to 5")
```

#### If-Elif-Else Statement

The `if-elif-else` statement is used for situations where a series of conditions are checked in order and the relevant code block is executed.

```python
x = 7

if x > 10:
    print("x is greater than 10")
elif x > 5:
    print("x is greater than 5 but less than or equal to 10")
else:
    print("x is less than or equal to 5")
```

### Examples

#### Temperature Status Check

```python
temperature = 25

if temperature > 30:
    print("It's hot")
elif temperature > 20:
    print("It's mild")
else:
    print("It's cool")
```

#### User Authorization

```python
username = "admin"
password = "12345"

input_username = input("Enter username: ")
input_password = input("Enter password: ")

if input_username == username and input_password == password:
    print("Login successful")
else:
    print("Invalid username or password")
```

These examples show how to use basic conditional statements. You can refer to Python documentation for more complex scenarios.

This guide can be used as the beginning of a section explaining basic conditional statements in your GitBook. You can expand the content by creating your own GitBook and adding more examples and explanations.

### Nested Conditional Statements

#### Example 1: Weather Check

```python
temperature = 28
humidity = 60

if temperature > 30:
    if humidity > 70:
        print("It's hot and humid, cooling down might be a good idea.")
    else:
        print("It's hot but humidity is low, it's a pleasant day!")
else:
    print("The weather is mild.")
```

In this example, the outer `if` condition checks the temperature, while the inner `if` condition checks the humidity. If the temperature is above 30 degrees and the humidity is also above 70, cooling down is recommended. Otherwise, if the temperature is high but the humidity is low, you can have a pleasant day.

#### Example 2: Student Grade Calculation

```python
grade = 75

if grade >= 90:
    print("Your grade is A")
elif grade >= 80:
    if grade >= 85:
        print("Your grade is B+")
    else:
        print("Your grade is B")
elif grade >= 70:
    if grade >= 75:
        print("Your grade is C+")
    else:
        print("Your grade is C")
else:
    print("Your grade is F")
```

In this example, letter grades corresponding to different grade ranges are calculated according to the student's grade. Using nested `if` and `elif` statements, specific grade ranges within certain limits are determined.

#### Example 3: User Authorization and Permission Check

```python
username = "admin"
password = "12345"
role = "admin"

input_username = input("Enter username: ")
input_password = input("Enter password: ")

if input_username == username and input_password == password:
    print("Login successful.")
    if role == "admin":
        print("Welcome to the admin panel.")
    else:
        print("Welcome to the standard user panel.")
else:
    print("Invalid username or password.")
```

In this example, if the username and password are correct and the user's role is "admin", the user logs into the admin panel. Otherwise, the user logs into the standard user panel.

These examples demonstrate how nested conditional statements can be used in a simple and understandable way. You can expand and use these basic structures for more complex scenarios.

\-----------------------------------------------------------------------------------------------------
