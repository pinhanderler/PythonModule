# Loops

In Python, loops are an important structure used to repeat a specific operation. Here are some examples explaining different types of loops:

### 1. `for` Loop

The `for` loop is used to iterate over a specific list, array, or array-like data structure.

#### Example 1: Printing List Elements

```python
colors = ["red", "blue", "green", "yellow"]

for color in colors:
    print(color)
```

#### Example 2: Summing Numbers

```python
numbers = [1, 2, 3, 4, 5]
total = 0

for num in numbers:
    total += num

print("Total:", total)
```

### 2. `while` Loop

The `while` loop is used to repeat an operation as long as a specific condition is true.

#### Example 3: Number Guessing Game

```python
import random

target_number = random.randint(1, 100)
guess = None

while guess != target_number:
    guess = int(input("Enter your guess: "))
    if guess < target_number:
        print("Guess a higher number.")
    elif guess > target_number:
        print("Guess a lower number.")
    else:
        print("Congratulations! Correct guess:", target_number)
```

#### Example 4: Factorial Calculation

```python
number = int(input("Enter the number whose factorial you want to calculate: "))
factorial = 1
i = 1

while i <= number:
    factorial *= i
    i += 1

print(f"Factorial of {number}:", factorial)
```

Loops are an important tool for repeating a specific task and processing data. The examples show how you can use `for` and `while` loops in different scenarios.

Nested loops mean using one loop inside another loop. Such loops are useful for creating more complex structures and processing data more deeply. Here are explanations and examples of nested loops:

### Nested `for` Loops

#### Example 1: Multiplication Table

```python
for i in range(1, 6):
    for j in range(1, 6):
        print(i * j, end="\t")
    print()
```

In this example, we create a multiplication table of numbers from 1 to 5. We print each multiplication result using two nested `for` loops.

### Nested `while` Loops

#### Example 2: Star Triangle

```python
size = 5
row = 1

while row <= size:
    col = 1
    while col <= row:
        print("*", end="")
        col += 1
    print()
    row += 1
```

In this example, we create a triangular pattern made of stars. We print the stars in the correct order using two nested `while` loops.

### Combined `for` and `while` Loops

#### Example 3: Matrix Transposition

```python
matrix = [[1, 2, 3],
          [4, 5, 6],
          [7, 8, 9]]

transposed = []

for i in range(len(matrix[0])):
    row = []
    for j in range(len(matrix)):
        row.append(matrix[j][i])
    transposed.append(row)

for row in transposed:
    print(row)
```

In this example, we calculate the transposition of a matrix. We convert the columns of the matrix to rows using nested `for` loops.

Nested loops are useful for creating more complex patterns or processing data more deeply. However, such loops can be more complex to understand and manage, so they should be used carefully and logically.

Infinite loops are situations where a loop runs continuously without ending based on a specific condition. Such loops usually arise from programmer errors and can cause programs to hang unintentionally. Let's examine an example of an infinite loop:

```python
while True:
    print("This is an infinite loop!")
```

In the example above, the `while True:` statement creates an infinite loop. Since the loop is always true, the code inside it will run continuously and the program will never be able to exit this loop. Such a loop causes the program to freeze.

To prevent infinite loops, it is important to set loop conditions correctly or use an appropriate exit mechanism inside the loop. For example:

```python
while True:
    user_input = input("Press 'q' to exit: ")
    if user_input == 'q':
        break
    else:
        print("Invalid input.")
```

In the example above, there is a loop that takes input from the user until the user presses "q". When the user presses "q", the loop is terminated with the `break` statement.

Avoiding infinite loops and controlling your loops in a logical way is important to ensure your program works correctly.

The `for` loop in Python is generally used to process items in a sequential data structure one by one. However, if a condition that ends the loop is not specified, the `for` loop can become an infinite loop. This situation is called a "for infinite loop".

Let's look at an example of an infinite `for` loop:

```python
for i in range(5):
    print("This is an infinite loop!")
```

Here, normally a `for` loop that iterates over numbers from 0 to 4 with the `range(5)` expression is expected. However, since there is no condition or exit mechanism inside the loop, this loop will run infinitely.

To avoid making this kind of error, it is important to set the loop condition correctly when using `for` loops and to provide a mechanism that ends the loop. For example:

```python
for i in range(5):
    user_input = input("Press 'q' to exit the loop: ")
    if user_input == 'q':
        break
    print(f"{i} operation completed.")
```

Here, if the user presses "q", the loop is terminated with the `break` statement. Otherwise, an operation is performed at each iteration.

Avoiding an infinite `for` loop and controlling your loops is important to ensure your program runs correctly and as expected.

`break` and `continue` are two keywords used to change the control flow in loops in Python. These two statements affect the behavior of loops and are used to stop or skip loops under certain conditions.

### `break` Statement

The `break` statement is used to suddenly terminate a loop. If a specific condition occurs, the loop ends immediately.

#### Example 1: Number Guessing Game

```python
target_number = 42

while True:
    guess = int(input("Enter your guess: "))
    if guess == target_number:
        print("Congratulations, correct guess!")
        break
    else:
        print("Wrong guess, try again.")
```

In this example, when the user makes the correct guess, the infinite `while` loop is terminated using the `break` statement.

### `continue` Statement

The `continue` statement is used to skip iterations that satisfy a specific condition inside a loop. When the condition is satisfied, the rest of the loop is skipped and the next iteration begins.

#### Example 2: Printing Even Numbers

```python
for i in range(1, 11):
    if i % 2 == 1:
        continue
    print(i, "is an even number.")
```

In this example, only even numbers are printed using the `continue` statement. Odd numbers are skipped and the loop moves to the next iteration.

The `break` and `continue` statements are useful tools for controlling flow based on specific conditions inside loops. However, overuse of these statements or creating a confusing code flow can make the code harder to understand. Therefore, they should be used carefully.
