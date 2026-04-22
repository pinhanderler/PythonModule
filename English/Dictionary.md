# Dictionaries

### What is a Dictionary?

In Python, a dictionary is a data structure that stores key-value pairs. Each key serves as an index that associates a value. Dictionaries are also called "maps", "hash tables", or "associative arrays" in many programming languages.

Key properties of dictionaries:

1. **Keys are Unique:** Each key can only appear once in a dictionary. Two pairs with the same key cannot be added.
2. **Mutable Data Structure:** Dictionaries can be dynamically updated with key-value pairs that are added, changed, or deleted.
3. **Unordered Data Structure:** From Python 3.7 and later versions, insertion order is preserved in dictionaries. However, the content of dictionaries is unordered and indexing cannot be used.

Dictionaries are useful for grouping or associating many different types of data. For example, you can store a person's name, age, and email address.

```python
person = {
    "name": "John",
    "age": 30,
    "email": "john@example.com"
}
```

In this example, the dictionary named `person` associates the keys "name", "age", and "email" with their respective values.

### How to Create a Dictionary?

There are different ways to create a dictionary in Python. Here are some of these methods:

**1. Creating a Dictionary with Curly Braces `{}`:**

```python
person = {
    "name": "Mike",
    "age": 60,
    "email": "mikejones@example.com"
}
```

With this method, you can create a dictionary by writing key-value pairs inside curly braces.

**2. Creating a Dictionary with the dict() Function:**

```python
person = dict(name="John", age=30, email="john@example.com")
```

You can create a dictionary by passing keys and values as arguments using the `dict()` function.

**3. Creating a Dictionary Using Lists and Tuples:**

```python
keys = ["name", "age", "email"]
values = ["John", 30, "john@example.com"]
person = dict(zip(keys, values))
```

You can create a dictionary by combining lists or tuples containing keys and values using the `zip()` function.

**4. Associating Keys with Values Using the fromkeys() Method:**

```python
keys = ["name", "age", "email"]
default_value = "N/A"
person = dict.fromkeys(keys, default_value)
```

The `fromkeys()` method allows you to create a dictionary that associates specified keys with a specified default value.

These methods show different ways to create dictionaries. Whichever method you use, keys must be unique and keys in dictionaries are stored in an unordered manner.

### Dictionary Examples:

Below are some examples of using values with different data types in a dictionary:

**1. Strings and Numbers:**

```python
person = {
    "name": "John",
    "age": 30,
    "email": "john@example.com"
}
```

**2. Lists and Tuples:**

```python
student = {
    "name": "Alice",
    "grades": [85, 90, 78, 95],
    "info": ("Computer Science", "Sophomore")
}
```

**3. Nested Dictionary:**

```python
school = {
    "name": "XYZ School",
    "location": "City A",
    "students": {
        "Alice": {
            "age": 16,
            "grade": 11
        },
        "Bob": {
            "age": 17,
            "grade": 12
        }
    }
}
```

**4. Bool and None:**

```python
settings = {
    "debug_mode": True,
    "logging": False,
    "api_key": None
}
```

**5. Mixed Data Types:**

```python
data = {
    "name": "Jane",
    "age": 28,
    "scores": [95, 88, 72],
    "info": {
        "city": "New York",
        "country": "USA"
    }
}
```

In these examples, you can see values with different data types inside a dictionary. Dictionaries are quite useful for grouping and associating different data types.

### Accessing Elements in a Dictionary

You can access elements in a Python dictionary using their keys. Here are examples of how to access elements in a dictionary:

```python
person = {
    "name": "John",
    "age": 30,
    "email": "john@example.com"
}

# Accessing elements using keys
name = person["name"]
age = person["age"]
email = person["email"]

print(name)   # John
print(age)    # 30
print(email)  # john@example.com
```

In this example, we use keys to access elements inside the dictionary. Pay attention to the following points when accessing values using keys:

1. If the specified key is not found in the dictionary, you will get a `KeyError` error. Therefore, it is good practice to check with the `in` keyword before accessing a non-existent key.

```python
if "address" in person:
    address = person["address"]
else:
    address = "N/A"
```

2. If you use the `get()` method instead of checking the key, you can return a default value you specify instead of getting an error for a non-existent key.

```python
address = person.get("address", "N/A")
```

This way, if the key doesn't exist, the `address` value will be "N/A".

### Adding an Element to a Dictionary or Updating an Existing Element

To add a new element to a dictionary in Python, you need to assign a new value associated with an existing key. Here are some methods you can use to add elements to a dictionary:

**1. Updating an Element with an Existing Key:**

```python
person = {
    "name": "John",
    "age": 30
}

person["age"] = 31  # Updating the value of the element with "age" key
```

**2. Adding a New Key and Value:**

```python
person = {
    "name": "John",
    "age": 30
}

person["email"] = "john@example.com"  # Adding a new key and value
```

**3. Adding an Element with setdefault() Method:**

```python
person = {
    "name": "John",
    "age": 30
}

person.setdefault("email", "john@example.com")  # Adds if "email" key doesn't exist
```

**4. Adding Multiple Elements with update() Method:**

```python
person = {
    "name": "John",
    "age": 30
}

new_data = {
    "email": "john@example.com",
    "city": "New York"
}

person.update(new_data)  # Adding multiple elements
```

### Other Dictionary Methods

Let's explain some important methods you can use for the dictionary data structure in Python with examples:

**1. keys():** Returns all keys in the dictionary as a list.

```python
person = {"name": "John", "age": 30, "email": "john@example.com"}
keys = person.keys()
print(keys)  # dict_keys(['name', 'age', 'email'])
```

**2. values():** Returns all values in the dictionary as a list.

```python
person = {"name": "John", "age": 30, "email": "john@example.com"}
values = person.values()
print(values)  # dict_values(['John', 30, 'john@example.com'])
```

**3. items():** Returns all key-value pairs in the dictionary as a list.

```python
person = {"name": "John", "age": 30, "email": "john@example.com"}
items = person.items()
print(items)  # dict_items([('name', 'John'), ('age', 30), ('email', 'john@example.com')])
```

**4. get():** Returns the value of the specified key. If the key doesn't exist, returns the specified default value.

```python
person = {"name": "John", "age": 30}
email = person.get("email", "N/A")
print(email)  # N/A
```

**5. pop():** Removes the element with the specified key and returns its value. If the key doesn't exist, returns the specified default value.

```python
person = {"name": "John", "age": 30}
email = person.pop("email", "N/A")
print(email)  # N/A
```

**6. popitem():** Removes the last added key-value pair and returns it as a tuple.

```python
person = {"name": "John", "age": 30, "email": "john@example.com"}
last_item = person.popitem()
print(last_item)  # ('email', 'john@example.com')
```

**7. clear():** Clears the dictionary content, leaving only an empty dictionary.

```python
person = {"name": "John", "age": 30}
person.clear()
print(person)  # {}
```

**8. copy():** Returns a copy of the dictionary.

```python
person = {"name": "John", "age": 30}
person_copy = person.copy()
```

These methods are some important tools you can use to process and manipulate the dictionary data structure.

### Dictionary Comprehensions

Dictionary comprehensions are a quick and compact way to create a new dictionary in Python. They work similarly to list comprehensions, but produce a dictionary as a result. Using dictionary comprehension, you can create key-value pairs from an existing iterable (list, tuple, etc.).

The dictionary comprehension structure is as follows:

```python
new_dict = {key_expression: value_expression for element in iterable}
```

Here are some examples:

**1. Squares Dictionary:**

```python
numbers = [1, 2, 3, 4, 5]
squares_dict = {num: num**2 for num in numbers}
print(squares_dict)  # {1: 1, 2: 4, 3: 9, 4: 16, 5: 25}
```

**2. Character Count Dictionary:**

```python
text = "hello world"
char_count_dict = {char: text.count(char) for char in text}
print(char_count_dict)  # {'h': 1, 'e': 1, 'l': 3, 'o': 2, ' ': 1, 'w': 1, 'r': 1, 'd': 1}
```

**3. Even Numbers Only Dictionary:**

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_dict = {num: num**2 for num in numbers if num % 2 == 0}
print(even_dict)  # {2: 4, 4: 16, 6: 36, 8: 64, 10: 100}
```

Using dictionary comprehension, you can perform more complex operations in a single line and group data in a different way.

### Checking Whether an Element is in the Dictionary

To check whether an element is in a Python dictionary, you can use the `in` keyword. Here is an example of how to do this:

```python
my_dict = {"key1": "value1", "key2": "value2", "key3": "value3"}

search_element = "key2"

if search_element in my_dict:
    print(f"{search_element} found in dictionary: {my_dict[search_element]}")
else:
    print(f"{search_element} not found in dictionary.")
```

### Iterating Through a Dictionary

You can use a `for` loop in Python to iterate over a dictionary. Here are two common methods you can use to access the keys or values of the dictionary:

1. Iterating over keys:

```python
my_dict = {"key1": "value1", "key2": "value2", "key3": "value3"}

for key in my_dict:
    value = my_dict[key]
    print(f"Key: {key}, Value: {value}")
```

2. Iterating over values:

```python
my_dict = {"key1": "value1", "key2": "value2", "key3": "value3"}

for value in my_dict.values():
    print(f"Value: {value}")
```

3. Iterating over both keys and values:

```python
my_dict = {"key1": "value1", "key2": "value2", "key3": "value3"}

for key, value in my_dict.items():
    print(f"Key: {key}, Value: {value}")
```

### Some Built-in Functions for Dictionaries:

1. `all()`: Returns `True` if all items in a given iterable return `True`; otherwise returns `False`.

```python
values = [True, True, False, True]
result = all(values)
print(result)  # Output: False
```

2. `any()`: Returns `True` if at least one item in a given iterable returns `True`; returns `False` if all items are `False`.

```python
values = [False, False, True, False]
result = any(values)
print(result)  # Output: True
```

3. `len()`: Returns the length of an iterable.

```python
my_list = [1, 2, 3, 4, 5]
length = len(my_list)
print(length)  # Output: 5
```

4. `sorted()`: Sorts an iterable and returns a sorted list.

```python
my_list = [4, 2, 1, 3, 5]
sorted_list = sorted(my_list)
print(sorted_list)  # Output: [1, 2, 3, 4, 5]
```
