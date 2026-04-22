# Variables

### Basic Concepts of Variables in Python

Variables are the fundamental building blocks used to store and process data. In Python, defining variables is quite simple. To define a variable, you need to specify a name and assign a value. Here is the basic usage:

```python
# Defining a variable and assigning a value
name = "Ahmet"
age = 25
pi = 3.14
```

In the example above, the variables `name`, `age`, and `pi` were assigned a string, an integer, and a decimal number respectively.

The properties of variables in Python are as follows:

### 1. Variable Names

When naming variables in Python, you need to follow certain rules. These rules ensure that your code is more readable and error-free. Here are the basic rules for variable naming in Python:

1. Variable names must start with a letter (A-Z or a-z) or an underscore (\_). They cannot start with a digit.
2. Names can contain letters (A-Z or a-z), digits (0-9), or underscores (\_).
3. Python is case-sensitive. So `name` and `Name` are different variable names.
4. Python reserved keywords cannot be used as variable names. For example `if`, `else`, `while`, `for`, `def`, etc.
5. Variable names should be meaningful and descriptive to help other developers better understand your code.
6. Names cannot contain spaces or special characters. Only letters, digits, and underscores are allowed.
7. For long variable names, naming styles like snake\_case or camelCase are preferred. snake\_case means writing words in lowercase separated by underscores. camelCase means the first word starts with a lowercase letter and subsequent words start with uppercase letters.

Examples:

```python
# Valid variable names
name = "Ahmet"
age = 25
grade_average = 85.5
total_person_count = 100

# Invalid variable names
5_years = 5       # Cannot start with a digit
if = 10           # Cannot use a keyword
first last = "Ali Veli"  # Cannot contain spaces
```

By following these rules when creating variable names, you ensure that your code is more readable and understandable.

Python reserved keywords are words that have special meanings and perform specific tasks. These keywords are the building blocks that define the syntax and semantics of the Python language and cannot be used as variable or function names. Here are the keywords that cannot be used in Python:

```python
False      class      finally    is         return
None       continue   for        lambda     try
True       def        from       nonlocal   while
and        del        global     not        with
as         elif       if         or         yield
assert     else       import     pass
break      except     in         raise
```

**Multi-Word Variable Names**

Yes, there are different approaches to creating a variable name with multiple words in Python. Here are two of them:

1. **Snake Case:** In this approach, you write words in lowercase and separate them with underscores (\_).

```python
grade_average = 85.5
student_full_name = "Ahmet Yılmaz"
```

2. **Camel Case:** In this approach, the first word starts with a lowercase letter, and subsequent words start with uppercase letters.

```python
gradeAverage = 85.5
studentFullName = "Ahmet Yılmaz"
```

Both approaches are valid and a matter of preference. However, the more common approach in the Python community is generally "snake\_case". This approach is used more widely and Python libraries, the standard library, and many resources are named this way.

Remember that whichever approach you use, it is important to create variable names that are meaningful, descriptive, and help other developers better understand your code.

### 2. Variable Types

In Python, the types of variables are determined automatically. That is, you do not need to specify the type. The basic data types are:

* `int` (integer)
* `float` (decimal number)
* `str` (string/text)
* `bool` (logical value - True or False)

Example:

```python
age = 25           # int
grade_average = 85.5  # float
name = "Ahmet"     # str
is_correct = True  # bool
```

### 3. Using Variables

**Assigning a Value to a Variable**

Assigning a value to a variable in Python is quite simple. After defining a variable, you can assign any value to it. Here are some examples:

1. **Assigning an Integer Value:**

```python
x = 10
```

2. **Assigning a Decimal Value:**

```python
pi = 3.14
```

3. **Assigning a String Value:**

```python
name = "Ahmet"
```

4. **Assigning a Boolean Value:**

```python
is_correct = True
```

5. **Assigning Value Between Variables:**

```python
x = 5
y = x  # Assigned the value of x to y
```

6. **Assigning Expression Results:**

```python
a = 5
b = 10
total = a + b  # You can assign the results of expressions
```

7. **Swapping Values:**

```python
x = 5
y = 10

x, y = y, x  # Swapped the values of variables x and y
```

**Assigning a Different Value to a Variable**

Changing the value of a variable in Python is quite easy. To update a variable with a new value, you can simply repeat the assignment. Here are some examples:

```python
x = 5
print("First value of x:", x)

x = 10  # Updated the value of x
print("Updated value of x:", x)

y = 2
y = y + 3  # Updated the value of variable y (new value: 5)
print("Updated value of y:", y)

z = 7
z += 1  # Incremented z by 1 (new value: 8)
print("Updated value of z:", z)
```

As seen in the examples above, to update the value of a variable, you simply need to make a new assignment. Also, you can increment or decrement a variable's value using short forms (e.g., `+=`, `-=`).

**Swapping Values with Multiple Variable Assignment:**

```python
x = 10
y = 5
x, y = y, x  # Swapped the values of variables x and y
```

This way, you can match and assign multiple variables and values in a single line. The important thing is that the number of variables matches the number of values. Otherwise you may get an error.

**Assigning Values to Multiple Variables in a Single Line**

Python allows you to assign values to multiple variables in a single line:

```python
a, b, c = 5, 3.2, "Hello"

print(a)
print(b)
print(c)
```

```
5
3.2
Hello
```

**Note:** Make sure that the number of variables matches the number of values, otherwise you will get an error.

**Assigning the Same Value to Multiple Variables at Once**

If we want to assign the same value to multiple variables at once, we can do it as follows:

```python
x = y = z = "same"

print(x)
print(y)
print(z)
```

```python
same
same
same
```

The program above assigns the same string to all of the variables x, y, and z.

You can perform mathematical operations using variables:

```python
a = 10
b = 5
total = a + b
product = a * b
quotient = a / b
```

\-----------------------------------------------------------------------------------------------------
