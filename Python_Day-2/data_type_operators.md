[![LinkedIn](https://img.shields.io/badge/Connect%20with%20me%20on-LinkedIn-blue.svg)](https://www.linkedin.com/in/rohit-rawat-7383091a7/)
[![GitHub](https://img.shields.io/github/stars/AmanPathak-DevOps.svg?style=social)](http://github.com/RohitRawat891997)
[![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)](https://app.docker.com/accounts/rohitrawat891997)

---

# 🐍 Python Basics — Day 2 Notes

---

## ▶️ Running Python & Importing Modules

```python
print("Hello")

import os
print(os.getcwd())
```

✅ `import os` → Loads Python's OS module
✅ `os.getcwd()` → Shows current working directory

---

# 📊 Data Types in Python

Python supports multiple built-in data types:

* `int`
* `float`
* `bool`
* `str`
* `complex`

---

## 🔢 Integer (`int`)

* Whole numbers
* Base-10 values (0-9)

```python
x = 10
```

---

## 🔣 Float (`float`)

* Decimal numbers

```python
price = 23.5
value = 7.99
```

---

## ✅ Boolean (`bool`)

```python
True   # value = 1
False  # value = 0
```

Used in conditions and logical operations.

---

## 🧵 String (`str`)

Different ways to write strings:

```python
'a'        # character / word
"hello"    # single line
'''multi line'''
"""multi line"""
```

### Escape Characters

```python
s="you can't do this"
```

```python
s='you can\'t do this'
print(s)
```

```python
s="you can\"t do this"
```

### Multiline String

```python
st='''line1
line2
line3'''
```

---

## 🔢 Complex Numbers

Format:

```
<real> + <imaginary>j
```

```python
x = 2 + 3j
type(x)
```

---

# 🧮 Python Operators

---

## 1️⃣ Arithmetic Operators

| Operator | Meaning                 |
| -------- | ----------------------- |
| `+`      | Addition                |
| `-`      | Subtraction             |
| `*`      | Multiplication          |
| `/`      | Division (float result) |
| `//`     | Floor Division          |
| `%`      | Modulus                 |
| `**`     | Power                   |

```python
x = 23
y = 4

# x + y
# x - y
# x * y
# 13 % 2
# 13 / 2
# 12 // 2
# 4 ** 3
```

---

## 2️⃣ Comparison Operators

Used to compare values.

```
== , != , > , < , >= , <=
```

```python
x = 90
y = 88

18 <= 18
```

---

## 3️⃣ Logical Operators

```
and , or , not
```

```python
not 20 > 3
```

---

## 4️⃣ Membership Operators

Check if a value exists inside a list or sequence.

```
in , not in
```

```python
users = ["amit","root","ram","rohan"]

"root" in users

data = ["Amit",34,23.7]
"amit" in data
```

---

## 5️⃣ Assignment Operators

```python
=   # assign value
+=  # add and assign
-=  # subtract and assign
```

Example:

```python
x = 2
x += 3   # same as x = x + 3
```

---

## 6️⃣ Identity Operators

Used to compare memory location.

```
is , is not
```

```python
a = 45
b = 45

a is b
```

### `id()` Function

Shows memory address of variable.

```python
id(a)
id(b)
```

```python
x == y   # compares value
x is y   # compares memory identity
```

---

# 🧪 Practice Questions (For Practice Only)

```
# Program to take input from the user (name and age).

# write a python program that takes your age as input and print:
* the value entered.
* its data type.

# program to input two numbers and print their sum:

# write a program that takes two numbers and prints:
* their sum, difference, and product
* whether the first number is greater than the second

Q- what are data types in python? list any 4 with examples.
Q- what is the difference between implicit and explicit type conversion
Q- what are operators in python? Explain any three types with examples.
```

---

# 👨‍💻 Author

**Name:** Rohit Rawat<br>
**GitHub:** [https://github.com/RohitRawat891997](https://github.com/RohitRawat891997)<br>
**LinkedIn:** [https://www.linkedin.com/in/rohit-rawat-7383091a7/](https://www.linkedin.com/in/rohit-rawat-7383091a7/)

---

