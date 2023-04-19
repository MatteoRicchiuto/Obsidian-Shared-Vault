Completed: Yes
Created: March 2, 2023
Tag: [[Python MOC]]

---

### Variables

In Python, a variable is an entity that is used to store a value or an instance of an object in memory. It is a name that refers to a reserved area of memory where a value is stored.

> [!Warning]
> In Python, it is **not necessary to declare the type of a variable** before using it, as the type is determined automatically during program execution. In other words, the type of the variable depends on the value that is assigned to it.

To define a variable in Python, you can use the following syntax:

```python
variable_name = value
```

Where `variable_name` is the name of the variable and `value` is the value that is assigned to the variable. 

---
## Naming Conventions

When naming variables in Python, there are some conventions that should be followed:

- The name of the variable should be descriptive and should represent what it is used for.
- The name of the variable should start with a lowercase letter.
- If the name of the variable contains multiple words, they should be separated by an underscore. For example, `my_variable`.
- Python has some reserved keywords that cannot be used as variable names, such as `if`, `else`, `while`, and `for`.

---

## Built-in Data Types

Variables can store data of different types, and different types can do 
different things.

Python has the following data types built-in by default, in these categories:

| Text Type: | str |
| --- | --- |
| Numeric Types: | int, float,complex |
| Sequence Types: | list, tuple, range |
| Mapping Type: | dict |
| Set Types: | set, frozenset |
| Boolean Type: | bool |
| Binary Types: | bytes, bytearray, memoryview |
| None Type: | NoneType |

| Example | Data Type |
| --- | --- |
| x = "Hello World" | str |
| x = 20 | int |
| x = 20.5 | float |
| x = 1j | complex |
| x = ["apple", "banana", "cherry"] | list |
| x = ("apple", "banana", "cherry") | tuple |
| x = range(6) | range |
| x = {"name" : "John", "age" : 36} | dict |
| x = {"apple", "banana", "cherry"} | set |
| x = frozenset({"apple", "banana", "cherry"}) | frozenset |
| x = True | bool |
| x = b"Hello" | bytes |
| x = bytearray(5) | bytearray |
| x = memoryview(bytes(5)) | memoryview |
| x = None | NoneType |

You can get the data type of any object by using the `type()` function:

```python
x = 5
print(type(x)) #Output: <class 'int'>
```

---

### Casting

There may be times when you want to specify a type on to a variable. 
This can be done with casting. Python is an object-orientated language, 
and as such it uses classes to define data types, including its 
primitive types.

Casting in python is therefore done using constructor functions:

- `int()` - constructs an integer number from an integer literal, a float literal (by removing all decimals), or a string literal (providing the string represents a whole number)
    
    ```python
    x = int(1)   # x will be 1
    y = int(2.8) # y will be 2
    z = int("3") # z will be 3
    ```
    
- `float()` - constructs a float number from an integer literal, a float literal or a string literal (providing the string represents a float or an integer)
    
    ```python
    x = float(1)     # x will be 1.0
    y = float(2.8)   # y will be 2.8
    z = float("3")   # z will be 3.0
    w = float("4.2") # w will be 4.2
    ```
    
- `str()` - constructs a string from a wide variety of data types, including strings, integer literals and float literals
    
    ```python
    x = str("s1") # x will be 's1'
    y = str(2)    # y will be '2'
    z = str(3.0)  # z will be '3.0
    ```
    

---