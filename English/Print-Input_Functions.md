# Print-Input Functions

## **Print Function**

The `print()` function in Python is a function used to print text or values to the console or output stream. This function is used for purposes such as monitoring the running state of your program, debugging, or interacting with the user. Here is the basic usage and examples of the `print()` function:

Basic usage:

```python
print("Hello, world!")
```

Usage with variables:

```python
name = "Ahmet"
age = 25
print("Hello,", name, ". You are", age, "years old.")
```

Printing different data types:

```python
number = 42
decimal_number = 3.14
text = "Python"
is_correct = True

print("Integer:", number)
print("Float:", decimal_number)
print("String:", text)
print("Boolean:", is_correct)
```

Printing outputs on the same line:

```python
print("Hello,", end=" ")
print("World!")
```

Printing multiple values together:

```python
name = "Ahmet"
age = 25
print("Hello,", name, ". You are", age, "years old.", sep="-")
```

As seen in these examples, the `print()` function takes texts and variables separated by commas. By default, each `print()` call is printed on a new line. However, you can change this behavior using the `end` parameter. Also, you can specify which character comes between values using the `sep` parameter.

The `print()` function is especially useful for seeing values and results during the development phase. It is a basic tool used for debugging and understanding the flow of the program.

**Parameters of the `print()` function:**

1. `objects`: Refers to the objects to be printed. Multiple objects can be written separated by commas. Example:

```python
name = "Ahmet"
age = 25
print("My name is", name, "and I am", age, "years old.")
# Output: My name is Ahmet and I am 25 years old.
```

2. `sep`: Specifies the separator character to be used between objects. Example:

```python
name = "Ahmet"
surname = "Yılmaz"
print(name, surname, sep="-")
# Output: Ahmet-Yılmaz
```

3. `end`: Specifies the character to be used at the end of the `print()` function. Example:

```python
print("Hello", end="!")  # Used exclamation mark instead of newline at the end
# Output: Hello!
```

4. The escape sequence is a special character sequence used in Python and many other programming languages. This sequence is used to start a new line in text or to make a line ending. It is not perceived as a character, but when found in text, it acts like a "new line" or "end of line" character.

For example:

```python
print("Hello,\nworld!")
```

This code will produce a two-line output:

```
Hello,
world!
```

You can use the `\n` escape sequence to split text into multiple lines or create more organized outputs.

These examples showed the different parameters and features of the `print()` function. You can customize outputs and adapt them to various scenarios using these parameters.

\-----------------------------------------------------------------------------------------------------

## **Taking Input**

To get input from the user in Python, you can use the `input()` function. This function waits for the user to enter text and returns the entered text as a string. Here is the usage of the `input()` function and an example:

Basic usage:

```python
user_input = input("Please enter some text: ")
print("The text you entered:", user_input)
```

In this example, the user is asked to enter text and the entered text is assigned to the `user_input` variable. Then, the entered text is printed to the screen.

Converting input to a number:

```python
age = input("Enter your age: ")
age_int = int(age)
print("In the future, you will be", age_int + 10, "years old.")

# Second way
age = int(input("Enter your age: "))
print("In the future, you will be", age + 10, "years old.")
```

After receiving the user's input, you can use the `int()` function to convert the value received as text to a number when needed. In this example, after the user enters their age, we calculate and print how old they will be in 10 years.

Converting input to a decimal number:

```python
height = input("Enter your height in meters: ")
height_float = float(height)
print("Double your height:", height_float * 2)
```

If you expect the user to enter a decimal number, you can convert the entered text to a decimal number using the `float()` function.

When taking user input, it is used to make the program wait. The program waits until the user types the entered text and presses the Enter key. After the input is received, the program continues.

When taking user inputs, you need to make sure that the input is of the correct type and that you handle errors. It is important to prevent your program from crashing or encountering errors if the user enters something different from what you expect.

\-----------------------------------------------------------------------------------------------------
