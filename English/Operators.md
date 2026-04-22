# Operators

In Python, operators are symbols or special words used to manipulate different types of data, perform calculations, or compare values. Operators are one of the fundamental building blocks of programming and are found in a wide range in Python as well. Here are some basic operator types commonly used in Python:

### 1. Arithmetic Operators

Arithmetic operators are used to perform mathematical calculations:

* `+`: Addition
* `-`: Subtraction
* `*`: Multiplication
* `/`: Division
* `%`: Modulus (finding the remainder)
* `**`: Exponentiation

Example:

```python
x = 10
y = 3

total = x + y
difference = x - y
product = x * y
quotient = x / y
remainder = x % y
power = x ** y
```

```python
x = 15
y = 4

# Output: x + y = 19
print('x + y =', x+y)

# Output: x - y = 11
print('x - y =', x-y)

# Output: x * y = 60
print('x * y =', x*y)

# Output: x / y = 3.75
print('x / y =', x/y)

# Output: x // y = 3
print('x // y =', x//y)

# Output: x ** y = 50625
print('x ** y =', x**y)
```

### 2. Comparison Operators

Comparison operators are used to compare values and create conditions:

* `==`: Is equal?
* `!=`: Is not equal?
* `<`: Is less than?
* `>`: Is greater than?
* `<=`: Is less than or equal?
* `>=`: Is greater than or equal?

Example:

```python
x = 5
y = 7

is_equal = x == y
is_less = x < y
is_greater = x > y
```

```python
x = 10
y = 12

# Output: x > y is False
print('x > y is', x>y)

# Output: x < y is True
print('x < y is', x<y)

# Output: x == y is False
print('x == y is', x==y)

# Output: x != y is True
print('x != y is', x!=y)

# Output: x >= y is False
print('x >= y is', x>=y)

# Output: x <= y is True
print('x <= y is', x<=y)
```

### 3. Logical Operators

Logical operators are used to manipulate logical values (True or False):

* `and`: Logical AND
* `or`: Logical OR
* `not`: Logical NOT

Example:

```python
a = True
b = False

result1 = a and b
result2 = a or b
result3 = not a
```

```python
x = True
y = False

print('x and y is', x and y)

print('x or y is', x or y)

print('not x is', not x)
```

```python
x and y is False
x or y is True
not x is False
```

`and` and `or` are logical operators that perform logical operations in Python. These operators are generally used in situations such as combining conditions or evaluating comparison expressions. Here are the differences between the `and` and `or` operators:

1. **and Operator:** This operator ensures that the result is true (True) when both conditions are true (True). That is, all conditions must be true.

   Example:

   ```python
   x = 5
   y = 10
   if x > 0 and y > 0:
       print("Both conditions are true.")
   ```

2. **or Operator:** This operator ensures that the result is true (True) when at least one condition is true (True). That is, it is sufficient for at least one condition to be true.

   Example:

   ```python
   x = 5
   y = -2
   if x > 0 or y > 0:
       print("At least one condition is true.")
   ```

In summary, the `and` operator results in true when all conditions are true, while the `or` operator ensures the result is true when at least one condition is true. These operators are quite useful for combining conditional expressions and making logical decisions.

### 4. Assignment Operators

Assignment operators are used to assign values to variables:

* `=`: Value assignment
* `+=`: Assignment with addition
* `-=`: Assignment with subtraction
* `*=`: Assignment with multiplication
* `/=`: Assignment with division
* `%=`: Assignment with modulus
* `**=`: Assignment with exponentiation

Example:

```python
x = 10
y = 3

x += y   # x = x + y
x -= y   # x = x - y
x *= y   # x = x * y
x /= y   # x = x / y
x %= y   # x = x % y
x **= y  # x = x ** y
```

These examples demonstrate the basic Python operators. Operators are a powerful tool that form the foundation of programming, and you can create more advanced programs with more complex operators and expressions.

\-----------------------------------------------------------------------------------------------------
