# String

String (text) is a data type used in computer programming and represents a sequence of characters. Strings are used to represent words, sentences, or any sequence of characters. Strings are an important data type in Python and many other programming languages, and are used in many areas such as text processing, data analysis, taking user input, reading/writing text-based files.

Strings are generally created by enclosing them in double quotes (`"..."`) or single quotes (`'...'`). Examples:

```python
name = "Ahmet"
surname = 'Yılmaz'
sentence = "Hello, world!"
```

You can perform various operations with strings, for example:

* You can concatenate strings:

  ```python
  full_name = name + " " + surname   # "Ahmet Yılmaz"
  ```
* You can create repetitions by multiplying strings:

  ```python
  repeated_text = name * 3  # "AhmetAhmetAhmet"
  ```
* You can measure the length of strings:

  ```python
  length = len(sentence)  # number of characters in sentence
  ```
* You can search for a specific character or substring within strings:

  ```python
  if "world" in sentence:
      print("The word 'world' is in sentence")
  ```
* You can slice strings:

  ```python
  sub_text = sentence[7:12]  # "world"
  ```

You can use indices to access characters in a string or perform operations on the string. Indices specify the order of characters in the string and increase starting from zero. Positive indices increase from left to right (starting from 0), negative indices increase from right to left (***starting from -1***).

For example, let's take the word "Merhaba":

```css
 M  e  r  h  a  b  a
 0  1  2  3  4  5  6
-7 -6 -5 -4 -3 -2 -1
```

In this table, the positive and negative indices of each character are shown.

You can use the index to access a specific character or character sequence in the text. Examples:

```python
text = "Merhaba"

first_char = text[0]    # "M"
second_char = text[1]   # "e"
last_char = text[-1]    # "a"
```

You can also use indices in slicing operations:

```python
sub_text = text[2:5]  # "rha"
```

This example takes a substring containing the characters from the 2nd index to the 5th index of the `text` variable.

You can perform many operations on strings with indices in Python. This is quite useful for taking parts of strings, manipulating substrings, and performing various operations on string data.

```python
str = "Holland"
print('str = ', str)  # Holland

# first character
print('str[0] = ', str[0])  # H

# last character
print('str[-1] = ', str[-1])  # d

# slicing characters between 2nd and 5th
print('str[1:5] = ', str[1:5])  # olla

# slicing last character between 6th and 2nd
print('str[5:-2] = ', str[5:-2])  # n
```

**Note:** When doing string slicing, it is used to obtain a substring consisting of the characters between the start and end indices of the slice. ***During the slicing operation, the start index is included while the end index is not included.***

For example, let's take the word "Merhaba":

```css
M  e  r  h  a  b  a
0  1  2  3  4  5  6
```

If the `text` variable is "Merhaba":

* The `text[1:4]` slice contains characters starting from the 1st index (e) up to the 4th index (h) (not included). The result is "erb".
* The `text[2:5]` slice contains characters starting from the 2nd index (r) up to the 5th index (a) (not included). The result is "rha".

The reason for this behavior is that indices generally start from 0 and counting the characters between indices is used to specify how many characters the slicing result will contain. Thus, while the start index of the slice is included, the end index is not included.

If only the start or end index is not specified, Python automatically slices from the beginning or to the end of the string. For example:

* The `text[:4]` expression contains characters from the beginning of the string to the 4th index (not included) since no start index is specified. The result is "Merh".
* The `text[3:]` expression contains characters starting from the 3rd index (h) to the end of the string since no end index is specified. The result is "haba".
* The `text[:]` expression contains the entire string since neither start nor end index is specified.

It is important to be careful that during the slicing operation, the start index is included while the end index is not included.

These are just basic string processing examples. There are many functions and methods in Python to perform more complex operations with strings, format strings, and perform string manipulation.

Python has a series of string methods for string manipulation. These methods are used to process, convert, and organize string data. Here are some commonly used Python string methods:

1. `len()`: Returns the length of a string. ***Note: len method starts from 1, it is different from index***

   ```python
   text = "Hello, world!"
   length = len(text)  # 13
   ```

2. `lower()`: Converts the string to lowercase.

   ```python
   text = "Hello, WORLD!"
   lowercase = text.lower()
   ```

3. `upper()`: Converts the string to uppercase.

   ```python
   text = "Hello, world!"
   uppercase = text.upper()
   ```

4. `capitalize()`: Makes the first letter of the string uppercase and leaves the rest lowercase.

   ```python
   text = "hello, world!"
   capitalized = text.capitalize()
   ```

5. `title()`: Makes the first letters of words uppercase.

   ```python
   text = "hello, world!"
   titled = text.title()
   ```

6. `strip()`: Removes leading and trailing spaces.

   ```python
   text = "   Hello, world!   "
   clean_text = text.strip()
   ```

7. `split()`: Splits the string according to a specific separator and returns a list.

   ```python
   text = "Hello,world,how are you?"
   words = text.split(",")
   ```

8. `replace()`: Replaces a specific substring with another substring.

   ```python
   text = "Hello, world!"
   new_text = text.replace("Hello", "Hi")
   ```

9. `find()`: Returns the position of a specific substring in the string.

   ```python
   text = "Hello, world!"
   position = text.find("world")
   ```

10. `startswith()`: Checks whether the string starts with a specific substring.

    ```python
    text = "Hello, world!"
    if text.startswith("Hello"):
        print("Starts!")
    ```

11. `endswith()`: Checks whether the string ends with a specific substring.

    ```python
    text = "Hello, world!"
    if text.endswith("world!"):
        print("Ends!")
    ```

These are just a few examples and there are many different string methods in Python. Using string methods, processing and organizing string data is quite easy.

\-----------------------------------------------------------------------------------------------------
