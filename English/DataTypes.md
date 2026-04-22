# Data Types

### Basic Data Types in Python

The basic data types used in Python with brief descriptions:

1. **Integer (int):** Represents all whole number values. For example: 1, -5, 1000.
2. **Float:** Represents decimal fractional numbers. For example: 3.14, -0.5.
3. **String (str):** Represents text or character sequences. For example: "Hello", 'Python', "123".
4. **Boolean (bool):** Represents true or false values. It has only two values: True or False.
5. **List (list):** Used to store multiple values in an ordered sequence. Can contain different types of data.
6. **Tuple:** Similar to a list, but values cannot be changed. Generally used to store fixed data.
7. **Dictionary (dict):** Used to store data with key-value pairs. Keys must be unique.
8. **Set:** Used to store unique and unordered data. Can perform operations like mathematical sets.
9. **Array:** Used to store and process numerical data in multi-dimensional arrays. Provided by the NumPy library.
10. **Comparable:** Used to store sortable data. It is not a special data type, but a concept used for sorting operations.

These basic data types are the most common and fundamental data types used in Python. Thanks to Python's flexible structure, you can combine these basic data types to create more complex structures.

In Python programming, various data types are used to represent different kinds of data. Data types play an important role in how the program works and how data is processed.

As a starting point, we will examine some of these data types.

### 1. Numeric Data Types

#### a. Integer (int)

Integers represent non-fractional numbers. Example:

```python
age = 25
student_count = 100
```

#### b. Float

Floats represent fractional numbers. Example:

```python
pi = 3.14
price = 19.99
```

### 2. Text Data Type

#### String (str)

The string data type represents text or character sequences. Strings can be defined within single quotes (`'`) or double quotes (`"`). Example:

```python
name = "Ahmet"
surname = 'Yılmaz'
```

### 3. Logical Data Type

#### Boolean (bool)

The boolean data type represents true (`True`) or false (`False`) values. It is generally used in conditional statements and decision structures. Example:

```python
is_correct = True
is_wrong = False
```

These data types are the most fundamental data types used in Python programming. However, there are also more complex data types, for example:

* **Lists**: Used to store multiple data in an ordered manner.
* **Tuples**: Similar to lists, but cannot be changed.
* **Dictionaries**: Stores data with key-value pairs.
* **Sets**: Used to store unique and unordered data.

You can refer to Python documentation and other resources to learn more about these data types and more complex topics.

To find out the type of a value in Python, you can use the `type()` function. This function returns the data type of an object (variable or value). Here is the usage of the `type()` function:

```python
x = 5
print(type(x))  # <class 'int'>

name = "Ahmet"
print(type(name))  # <class 'str'>

pi = 3.14
print(type(pi))  # <class 'float'>

is_correct = True
print(type(is_correct))  # <class 'bool'>
```

In this example, the `type()` function returns that the `x` variable belongs to the integer (`int`) data type, the `name` variable belongs to the string (`str`) data type, etc. This allows you to determine the type of a value and use it while developing your program.

Changing the data type of a variable in Python is generally done through a conversion operation. This means converting an existing value to another data type. Python has some functions for data type conversion. Here are some examples:

1. **Converting to Integer (int):**

```python
number = "123"
number_int = int(number)
print(number_int)  # 123
```

2. **Converting to Float:**

```python
decimal_number = "3.14"
decimal_float = float(decimal_number)
print(decimal_float)  # 3.14
```

3. **Converting to String (str):**

```python
number = 123
number_str = str(number)
print(number_str)  # "123"
```

4. **Boolean Conversion (bool):**

```python
number = 0
number_bool = bool(number)
print(number_bool)  # False
```

Conversion operations should be performed carefully considering the compatibility between data types. For example, it is possible to convert a value that contains only digits in a string to an integer, but if the string contains letters, the conversion may give an error.

\-----------------------------------------------------------------------------------------------------
