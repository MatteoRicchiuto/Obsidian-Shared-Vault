Status: #Complete
Created: June 14, 2023
Tag: [[Python MOC]], [[Python Iterators, __iter__ and __next__]]

---
**Index:**
1. [[Python zip() Function#Definition|Definition ]]
2. [[Python zip() Function#Syntax|Syntax]]
3. [[Python zip() Function#Parameter Values|Parameter Values]]
4. [[Python zip() Function#Return Values|Return Values]]
5. [[Python sorted() Function#key Parameter in Python sorted() function|Key Parameter]]

---
## Definition 
The `sorted()` function sorts the elements of a given [[Python Iterators, __iter__ and __next__|iterable]] in a specific order (ascending or descending) and returns it as a list.

---
## Syntax
`sorted(iterable, key=None, reverse=False)`

---
## Parameter Values

|Parameter|Description|
|---|---|
|*iterable*| Iterator objects that will be joined together |
|*reverse (Optional)*|If `True`, the sorted list is reversed (or sorted in descending order). Defaults to `False` if not provided.|
|*key (Optional)* | A function that serves as a key for the sort comparison. Defaults to `None`. |

**Recommended Reading:** [[Python Iterators, __iter__ and __next__]]

---
## Return Values

The `sorted()` function returns a sorted list.

**Example 1) Sort string, list, and tuple;**
```python
# vowels list
py_list = ['e', 'a', 'u', 'o', 'i']
print(sorted(py_list)) 
# Output: ['a', 'e', 'i', 'o', 'u']

# string
py_string = 'Python'
print(sorted(py_string)) 
# Output: ['P', 'h', 'n', 'o', 't', 'y']


# vowels tuple
py_tuple = ('e', 'a', 'u', 'o', 'i') 
# Output: ['P', 'h', 'n', 'o', 't', 'y']

print(sorted(py_tuple))
```

**Notice:** that in all cases that a sorted list is returned.
> [!Note:] 
> A list also has the [[Python List sort() Method]] which performs the same way as `sorted()`. The only difference is that the `sort()` method doesn't return any value and changes the original list.

**Example 2) Sort in descending order:**

The `sorted()` function accepts a `reverse` parameter as an optional argument.

Setting `reverse = True` sorts the iterable in the descending order.
```python
# set
py_set = {'e', 'a', 'u', 'o', 'i'}
print(sorted(py_set, reverse=True))
# Output: ['u', 'o', 'i', 'e', 'a']

# dictionary
py_dict = {'e': 1, 'a': 2, 'u': 3, 'o': 4, 'i': 5}
print(sorted(py_dict, reverse=True))
# Output: ['u', 'o', 'i', 'e', 'a']

# frozen set
frozen_set = frozenset(('e', 'a', 'u', 'o', 'i'))
print(sorted(frozen_set, reverse=True))
# Output: ['u', 'o', 'i', 'e', 'a']
```

---
## key Parameter in Python sorted() function

If you want your own implementation for sorting, `sorted()` also accepts a `key` function as an optional parameter.

Based on the returned value of the key function, you can sort the given iterable.
```python
sorted(iterable, key=len)
```
Here, `len()` is Python's in-built function to count the length of an object.

The list is sorted based on the length of the element, from the lowest count to highest.

**Example:**
``` python
# take the second element for sort
def take_second(elem):
    return elem[1]


# random list
random = [(2, 2), (3, 4), (4, 1), (1, 3)]

# sort list with key
sorted_list = sorted(random, key=take_second)

# print list
print('Sorted list:', sorted_list)
# Output: Sorted list: [(4, 1), (2, 2), (1, 3), (3, 4)]
```