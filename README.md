# everything-i-learned-since-day-0-of-python

#  data types

# string data type

name ="prabha"
print("name")
#output = prabha

# combining strings

name="sister"
print("hello"+name)
output="hello sister"

# check data type 

name="prab"
print(type(name))

 output=<class'str'>

 # combine variable of same datatype
 first_name= "prabha"
 last_name = "sapkota"
 full_name= first_name + last_name
 print("hello"+ full_name)

 output = hello prabha sapkota

 # integer data type

 #no quotation, having one makes it a string

 age= 20
 age = age+1
 print(age+1)

 output= 21

 # float datatype

 #it is a numeric value which stores decimal

height = 250.5 
print (height)

   output= 250.5

  #if we have to typecast it,
  
  height = 250.5 
  print("height is:" str(height)+ "cm")
  output= 250.5cm
  
  # boolean value 
  #either TRUE or FALSE
  human = false
  print(human)
  output= FALSE

  #typecast it
  human = true
  print("are you human?" str(human))




# Multiple Assignment in Python

## What is Multiple Assignment?

**Multiple assignment** allows assigning values to multiple variables in a **single line of code**.

Python automatically matches values on the right to variables on the left.

---

## Basic Example

```python
a, b, c = 1, 2, 3
```

This is equivalent to:

```python
a = 1
b = 2
c = 3
```

---

## Swapping Values

Python allows swapping values without using a temporary variable.

```python
x = 5
y = 10

x, y = y, x
print(x, y)
```

Output:

```
10 5
```

---

## Assigning the Same Value to Multiple Variables

```python
x = y = z = 0
```

All variables receive the same value.

---

## Unpacking from Lists and Tuples

```python
values = [10, 20, 30]
a, b, c = values
```

```python
point = (4, 7)
x, y = point
```

---

## Ignoring Values Using `_`

```python
data = (1, 2, 3, 4)
a, b, _, _ = data
```

Useful when you don’t need all values.

---

## Multiple Assignment with User Input

```python
x, y = input("Enter two numbers: ").split()
x = int(x)
y = int(y)
```

---

## Common Errors

### Mismatch in number of values

```python
a, b = 1, 2, 3
```

### Too few values

```python
a, b, c = [1, 2]
```

Both raise errors.

---

## Practice Example

```python
a, b, c = 2, 4, 6
b, c = c, b
print(a, b, c)
```

---







# Lists in Python

## What is a List?

A **list** stores multiple values in a single variable.

```python
items = [10, 20, 30]
```

Lists are:

* ordered
* mutable (can change)
* allow duplicates

---

## Accessing Elements

```python
items[0]
items[-1]
```

---

## Modifying Elements

```python
items[1] = 50
```

---

## Adding Elements

```python
items.append(40)
items.insert(1, 99)
```

---

## Removing Elements

```python
items.remove(20)
items.pop()
items.pop(0)
```

---

## List Length

```python
len(items)
```

---

## Looping Through a List

```python
for item in items:
    print(item)
```

With index:

```python
for i in range(len(items)):
    print(i, items[i])
```

---

## Slicing

```python
items[1:3]
items[:2]
items[2:]
```

---

## Checking Membership

```python
if 30 in items:
    print("Found")
```

---

## Practice Example

```python
numbers = []

for i in range(5):
    numbers.append(int(input("Enter number: ")))

print(numbers)
print(max(numbers))
print(sum(numbers) / len(numbers))
```

---

## File Name

```
lists.py
```

 

# Loops in Python

## What is a Loop?

A **loop** is used to repeat a block of code multiple times.

---

## `for` Loop

Used to iterate over a sequence.

```python
for i in range(5):
    print(i)
```

---

## Looping Through a List

```python
numbers = [10, 20, 30]

for n in numbers:
    print(n)
```

---

## `range()` Function

```python
range(5)        # 0 to 4
range(1, 6)     # 1 to 5
range(1, 10, 2) # step of 2
```

---

## `while` Loop

Runs while a condition is true.

```python
i = 0
while i < 5:
    print(i)
    i += 1
```



## `break`

Stops the loop.

```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

---

## `continue`

Skips current iteration.

```python
for i in range(5):
    if i == 2:
        continue
    print(i)
```

---

## Nested Loops

```python
for i in range(3):
    for j in range(2):
        print(i, j)
```

---

## Common Mistake

Infinite loop:

```python
while True:
    print("Loop")
```

---

## Practice

```python
numbers = []

for i in range(5):
    numbers.append(int(input("Enter number: ")))

for n in numbers:
    if n % 2 == 0:
        print(n)
```

---



## FUNCTIONS IN PYTHON

### What is a Function?

A **function** is a reusable block of code that performs a specific task.

```python
def greet():
    print("Hello, Python!")
```

---

### Calling a Function

```python
greet()
```

---

### Why Use Functions?

* Reuse code
* Reduce repetition
* Improve readability
* Easier debugging and testing
* Foundation for OOP, DSA, Django, and backend development

---

## Syntax

```python
def function_name(parameters):
    # code
    return value
```

---

## Parameters and Arguments

```python
def add(a, b):      # parameters
    return a + b

add(3, 5)          # arguments
```

---

## Return Statement

```python
def square(n):
    return n * n
```

---

## Default Parameters

```python
def greet(name="Guest"):
    print(f"Hello {name}")
```

---

## Keyword Arguments

```python
def intro(name, age):
    print(name, age)

intro(age=17, name="Prabha")
```

---

## *args (Variable-Length Arguments)

```python
def total(*nums):
    return sum(nums)

print(total(1, 2, 3, 4))
```

---

## **kwargs (Keyword Variable-Length Arguments)

```python
def profile(**data):
    print(data)

profile(name="Prabha", course="Engineering")
```

---

## Scope (Local vs Global)

```python
x = 10

def test():
    x = 5
    print(x)

test()
print(x)
```

---

## Docstrings

```python
def multiply(a, b):
    """Returns the product of two numbers"""
    return a * b
```

---

## Lambda Functions

```python
square = lambda x: x * x
print(square(4))
```

---

## Practice Tasks

* Function to check even or odd
* Function to find the maximum of three numbers
* Function to count vowels in a string
* Function to calculate BMI

---

### **List Comprehension in Python 

**List comprehension** is a compact way to create lists using a single line of code instead of loops.

---

## Basic Syntax

```python
[expression for item in iterable]
```

---

## Simple Example

```python
squares = [x*x for x in range(5)]
```

Creates:

```
[0, 1, 4, 9, 16]
```

---

## With Condition

```python
evens = [x for x in range(10) if x % 2 == 0]
```

---

## With `if–else`

```python
labels = ["even" if x % 2 == 0 else "odd" for x in range(5)]
```

---

## Nested List Comprehension

```python
matrix = [[i*j for j in range(3)] for i in range(3)]
```

---

## Why Use It

* Cleaner than loops
* Faster execution
* Common in AI/ML data preprocessing

---

## Avoid When

* Logic becomes hard to read
* Multiple nested conditions

---

## One-Line Summary

> List comprehension = **loop + condition + list creation in one line**

