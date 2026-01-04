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


   

 
 
 


