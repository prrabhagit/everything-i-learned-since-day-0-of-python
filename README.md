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

A **list** is used to store multiple values in one variable.

```python
items = [10, 20, 30]
```

Lists are:

* ordered
* changeable
* allow duplicates

---

## Accessing Elements

```python
items[0]
items[-1]
```

---

## Changing Values

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


 
 
 


