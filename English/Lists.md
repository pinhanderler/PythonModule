# Lists

## What is a List?

In Python, the "list" data type is a data structure used to store multiple values and provide access to those values. Lists can contain different data types (for example, numbers, strings, other lists, etc.) and these values can be accessed through indices.

You can use square brackets `[]` to create a list. For example:

```python
my_list = [1, 2, 3, 4, 5]
```

This example creates a list containing numbers from 1 to 5.

Since lists are mutable, their contents can be changed at later stages of the program.

### How to Create a List?

In Python, you need to use square brackets `[]` to create a list. Here are examples showing you how to create lists in different ways:

1. **Creating an Empty List:**

```python
empty_list = []
```

2. **Creating a List with Elements:**

```python
numbers = [1, 2, 3, 4, 5]
fruits = ["apple", "banana", "orange"]
mixed_list = [1, "apple", True, 3.14]
```

3. **Creating a List Using the `list()` Function:**

```python
numbers = list([1, 2, 3, 4, 5])
```

4. **Creating a List Using the `range()` Function:**

```python
number_range = list(range(1, 6))  # List containing numbers from 1 to 5 (5 not included).
```

5. **Creating a List with List Comprehension:**

```python
squared_numbers = [x**2 for x in range(1, 6)]  # List containing squares of numbers from 1 to 5.
```

6. **Creating a List with Repeated Elements Using the `*` Operator:**

```python
repeated_list = ["hello"] * 3  # List containing "hello" three times.
```

These examples show you how to create lists in different ways. Since lists are mutable, you can update their contents later.

#### What is a Nested List?

A nested list is a list structure that contains other lists within a list. This is used to organize data hierarchically and create more complex data structures. Here are some examples:

**Example 1: Matrix Representation**

```python
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]
```

This example represents a 3x3 matrix. Each inner list represents a row of the matrix.

**Example 2: Student Information**

```python
students = [
    ["Alice", 23, "Computer Science"],
    ["Bob", 21, "Mathematics"],
    ["Eve", 22, "Physics"]
]
```

This example represents student information with nested lists. Each inner list contains a student's name, age, and department.

**Example 3: Movie List**

```python
movie_list = [
    ["The Matrix", 1999, ["Keanu Reeves", "Laurence Fishburne"]],
    ["Inception", 2010, ["Leonardo DiCaprio", "Joseph Gordon-Levitt"]],
    ["Jurassic Park", 1993, ["Sam Neill", "Laura Dern"]]
]
```

This example represents movie information with nested lists. Each inner list contains a movie's name, release year, and lead actors.

**Example 4: Tic Tac Toe Game Board**

```python
tic_tac_toe = [
    ["X", "O", "X"],
    ["O", "X", "O"],
    ["X", "X", "O"]
]
```

This example represents a Tic Tac Toe game board with nested lists. Each inner list represents the state of a row.

Nested lists can be very useful in situations where data needs to be organized and processed in more complex ways.

## How to Access an Element in a List?

In Python, you can use indices to access a specific element in a list. In lists, indices start from 0, meaning the first element of the list has index 0, the second element has index 1, and so on. Here are some examples:

```python
my_list = [10, 20, 30, 40, 50]

first_element = my_list[0]   # Gets the first element of the list (10).
second_element = my_list[1]  # Gets the second element of the list (20).
third_element = my_list[2]   # Gets the third element of the list (30).
```

Also, you can count backwards from the end of the list using negative indices:

```python
last_element = my_list[-1]        # Gets the last element of the list (50).
second_last_element = my_list[-2]  # Gets the second-to-last element (40).
```

If you want to access elements in a specific range, you can use the slicing method:

```python
sub_list = my_list[1:4]  # Sub-list containing elements from index 1 to index 3.
```

This way, you can access elements in a specific range of the list. Remember that indices are not inclusive of the boundary, meaning the `sub_list` in the example above actually contains elements from index 1 to index 3 (index 3 not included).

#### How to Access an Element in a Nested List?

Below you can find an example of a nested list and examples of how to access a specific element in this nested list:

```python
nested_list = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]

# Examples of accessing the nested list
element_1_1 = nested_list[1][1]  # Second element of the second row (5)
element_0_2 = nested_list[0][2]  # Third element of the first row (3)
element_2_0 = nested_list[2][0]  # First element of the third row (7)

print(element_1_1)  # Output: 5
print(element_0_2)  # Output: 3
print(element_2_0)  # Output: 7
```

In the example above, the expression `nested_list[1][1]` accesses the second row (index 1) of the nested list and the second element (index 1), so the result is `5`.

### Adding / Removing Elements from a List and Changing an Existing Element:

You can use various methods and methods to add and remove elements from a Python list. Here are some basic methods you can use:

**Adding Elements:**

1. **`append()` Method:** You can use the `append()` method to add a new element to the end of the list.

   ```python
   my_list = [1, 2, 3]
   my_list.append(4)  # Adds 4 to the end of the list.
   ```

2. **`insert()` Method:** You can use the `insert()` method to add a new element at a specific index.

   ```python
   my_list = [1, 2, 3]
   my_list.insert(1, 5)  # Adds 5 at index 1.
   ```

3. **`extend()` Method:** You can use the `extend()` method to merge one list with another and add elements.

   ```python
   my_list = [1, 2, 3]
   new_elements = [4, 5, 6]
   my_list.extend(new_elements)  # Adds [4, 5, 6] to the end of the list.
   ```

**Removing Elements:**

1. **`pop()` Method:** You can use the `pop()` method to remove an element at a specific index. If no index is specified, the last element is removed.

   ```python
   my_list = [1, 2, 3, 4, 5]
   popped_element = my_list.pop(2)  # Removes the third element (3) and returns it.
   ```

2. **`remove()` Method:** You can use the `remove()` method to remove the first element with a specific value.

   ```python
   my_list = [1, 2, 3, 2, 4]
   my_list.remove(2)  # Removes the first element with value 2.
   ```

3. **Removing by Value:** If you know the value of the element to be removed, you can remove it directly with `remove()` without using an index.

   ```python
   my_list = [1, 2, 3, 4, 5]
   my_list.remove(3)  # Removes the element with value 3.
   ```

4. **Removing with `del` Keyword:** You can use the `del` keyword to remove an element at a specific index.

   ```python
   my_list = [1, 2, 3, 4, 5]
   del my_list[1]  # Removes the second element (index 1).
   ```

5. **Deleting the List with `del` Keyword:**

   ```python
   my_list = [1, 2, 3, 4, 5]
   del my_list  # Deletes the entire list.
   # print(my_list)  # Error! my_list is no longer defined.
   ```

**Changing an element in a list:**

```python
my_list = [1, 2, 3, 4, 5]
my_list[0] = 10  # Changes the first element to 10.
# print(my_list)  # Result: [10, 2, 3, 4, 5]
```

Remember that when you remove an element from a list, the list is automatically reorganized and the indices are updated.

### List Methods

Here we can explain some common list methods used when working with lists in Python with examples:

1. **append()**: Adds an element to the end of the list.

```python
my_list = [1, 2, 3]
my_list.append(4)
# Result: [1, 2, 3, 4]
```

2. **extend()**: Adds the elements of another list to the end of a list.

```python
my_list = [1, 2, 3]
new_elements = [4, 5, 6]
my_list.extend(new_elements)
# Result: [1, 2, 3, 4, 5, 6]
```

3. **insert()**: Adds an element at a specific index.

```python
my_list = [1, 2, 3]
my_list.insert(1, 5)
# Result: [1, 5, 2, 3]
```

4. **remove()**: Removes the first element with a specific value.

```python
my_list = [1, 2, 3, 2, 4]
my_list.remove(2)
# Result: [1, 3, 2, 4]
```

5. **pop()**: Removes the element at a specific index and returns the removed element.

```python
my_list = [1, 2, 3, 4, 5]
popped_element = my_list.pop(2)
# Result: my_list = [1, 2, 4, 5], popped_element = 3
```

6. **clear()**: Removes all elements inside a list and makes the list empty.

```python
my_list = [1, 2, 3, 4, 5]
my_list.clear()  # Clears all elements.
print(my_list)   # Output: []
```

7. **index()**: Returns the index of the first element with a specific value.

```python
my_list = [10, 20, 30, 20, 40]
index = my_list.index(20)
# Result: index = 1
```

8. **count()**: Counts how many times a specific value appears in the list.

```python
my_list = [10, 20, 30, 20, 40]
count = my_list.count(20)
# Result: count = 2
```

9. **sort()**: Sorts the list from smallest to largest (makes a permanent change to the list).

```python
my_list = [4, 1, 3, 2]
my_list.sort()
# Result: my_list = [1, 2, 3, 4]
```

10. **reverse()**: Reverses the list (makes a permanent change to the list).

```python
my_list = [1, 2, 3, 4]
my_list.reverse()
# Result: my_list = [4, 3, 2, 1]
```

11. **copy()**: Creates a copy of the list.

```python
my_list = [1, 2, 3]
new_list = my_list.copy()
# Result: new_list = [1, 2, 3]
```

12. **len():** Returns the number of elements in the list.

```python
my_list = [1, 2, 3]
length = len(my_list)
# Result: 3
```

13. **sorted():** Sorts the items in a list and returns a sorted list.

```python
my_list = [4, 2, 1, 3, 5]
sorted_list = sorted(my_list)
print(sorted_list)  # Output: [1, 2, 3, 4, 5]
```

These are just some basic list methods. Python documentation or other resources can provide information about more list methods and details.

### List Comprehensions

List comprehensions are a structure in Python that allows a list to be created in a shorter and more readable way. List comprehensions allow you to create a new list by performing loop operations on an existing list, array, or data set.

List comprehensions are generally structured as follows:

```python
new_list = [expression for item in iterable if condition]
```

* `expression`: The expression of the new element to be created.
* `item`: Each item in the iterable (for example, list, array, or range).
* `iterable`: The data structure to be looped over.
* `condition` (optional): Used to filter elements based on a condition.

To explain with examples:

**Example 1: Squares List**

```python
numbers = [1, 2, 3, 4, 5]
squared_numbers = [x ** 2 for x in numbers]
# squared_numbers: [1, 4, 9, 16, 25]
```

**Example 2: Filtering Even Numbers**

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_numbers = [x for x in numbers if x % 2 == 0]
# even_numbers: [2, 4, 6, 8, 10]
```

**Example 3: Creating a Character Array**

```python
word = "Python"
letters = [char for char in word]
# letters: ['P', 'y', 't', 'h', 'o', 'n']
```

**Example 4: Nested List Comprehension**

```python
matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
flattened = [num for row in matrix for num in row]
# flattened: [1, 2, 3, 4, 5, 6, 7, 8, 9]
```

List comprehensions not only make your code shorter and more understandable, but also allow you to perform loop operations and element selections in a single line.

#### Querying Whether an Element is in the List

It is possible for us to query whether elements are in a list or not. For example:

```python
my_list = ['p', 'r', 'o', 'b', 'l', 'e', 'm']

# Output: True
print('p' in my_list)

# Output: False
print('a' in my_list)

# Output: True
print('c' not in my_list)
```
