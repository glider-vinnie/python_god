# Comprehensive Python Notes

> These notes cover Python essentials, from basic data structures like arrays and dictionaries to advanced topics like trees and graphs. Keywords and commonly used functions are included for reference. All code and concepts are beginner-friendly.

---

## 📌 Table of Contents
- [Data Types](#data-types)
- [Lists](#lists)
- [Tuples](#tuples)
- [Dictionaries](#dictionaries)
- [Sets](#sets)
- [Frozenset](#frozenset)
- [Arrays (via `array` module)](#arrays)
- [Strings](#strings)
- [List Comprehensions](#list-comprehensions)
- [Functions](#functions)
- [Function Arguments: `*args`, `**kwargs`](#function-arguments)
- [Lambda, Map, Filter, Reduce](#lambda-map-filter-reduce)
- [Classes & Objects](#classes--objects)
- [File Handling](#file-handling)
- [JSON Handling](#json-handling)
- [Recursion](#recursion)
- [Stacks & Queues](#stacks--queues)
- [Linked Lists](#linked-lists)
- [Trees](#trees)
- [Graphs](#graphs)
- [Useful Built-in Functions](#useful-built-in-functions)

---

## Data Types
- `int`, `float`, `complex` – numbers
- `bool` – `True` or `False`
- `str` – text
- `list`, `tuple`, `dict`, `set`, `frozenset`
- `bytes`, `bytearray`, `memoryview`
- `NoneType` – `None`

```python
a = 10            # int
b = 3.14          # float
c = 2 + 3j        # complex
flag = True       # bool
```

---

## Lists
> A dynamic array that can hold items of different data types.
```python
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")       # Add at end
fruits.pop()                  # Remove from end
fruits[0] = "mango"           # Change value at index 0
```
**Useful Methods:** `append()`, `pop()`, `insert()`, `remove()`, `reverse()`, `sort()`

## Tuples
> An immutable list - you cannot change its content after creation.
```python
t = (1, 2, 3)
print(t[0])
```
**Why Tuples?** Faster than lists, great for fixed data like coordinates.

## Dictionaries
> Stores data in key-value pairs.
```python
person = {"name": "Alice", "age": 25}
print(person["name"])
person["age"] = 26
```
**Useful Methods:** `get()`, `keys()`, `values()`, `items()`, `update()`

### Nested Dictionary
```python
students = {
  "101": {"name": "Alice", "score": 95},
  "102": {"name": "Bob", "score": 88}
}
print(students["101"]["name"])
```

## Sets
> Unordered collection of unique elements.
```python
s = {1, 2, 3}
s.add(4)
s.remove(1)
```

## Frozenset
> Immutable version of a set.
```python
fs = frozenset([1, 2, 3])
```

## Arrays
```python
import array
arr = array.array('i', [1, 2, 3, 4])
```

## Strings
```python
s = "Hello World"
print(s.lower())
print(s[0:5])
```

## List Comprehensions
```python
squares = [x*x for x in range(5)]
evens = [x for x in range(10) if x % 2 == 0]
```

## Functions
```python
def greet(name):
    return f"Hello {name}"
```

## Function Arguments
```python
def test_args(*args, **kwargs):
    print(args)
    print(kwargs)

test_args(1, 2, 3, name="Alice")
```

## Lambda, Map, Filter, Reduce
```python
square = lambda x: x*x
list(map(lambda x: x*x, [1, 2, 3]))
list(filter(lambda x: x > 2, [1, 2, 3]))
from functools import reduce
reduce(lambda x, y: x + y, [1, 2, 3])
```

## Classes & Objects
```python
class Dog:
    def __init__(self, name):
        self.name = name
    def bark(self):
        print(f"{self.name} says woof!")
```

## File Handling
```python
with open("file.txt", "w") as f:
    f.write("hello")
```

## JSON Handling
```python
import json
json_data = '{"name": "Alice", "age": 25}'
parsed = json.loads(json_data)
print(parsed["name"])
```

## Recursion
```python
def factorial(n):
    if n == 0: return 1
    return n * factorial(n-1)
```

## Stacks & Queues
```python
# Stack
stack = []
stack.append(1)
stack.pop()

# Queue
from collections import deque
queue = deque()
queue.append(1)
queue.popleft()
```

## Linked Lists
```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
```

## Trees
```python
class TreeNode:
    def __init__(self, val):
        self.val = val
        self.left = None
        self.right = None

def inorder(root):
    if root:
        inorder(root.left)
        print(root.val)
        inorder(root.right)
```

## Graphs
```python
graph = {
  'A': ['B', 'C'],
  'B': ['D'],
  'C': ['E'],
  'D': [],
  'E': []
}
```

## Useful Built-in Functions
```python
len(), type(), range(), enumerate(), zip(), any(), all(), abs(), bin(), chr(), dir(), divmod(), filter(), hex(), id(), iter(), max(), min(), next(), oct(), pow(), repr(), round(), sorted(), sum(), vars()
```

---

> 📘 Tip: For advanced structures, check `heapq`, `collections`, `bisect`, and `networkx`.

> ✅ Beginner-friendly and ready for college, interviews, and GitHub! 🎓
