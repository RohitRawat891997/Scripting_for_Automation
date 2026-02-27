## 🌐 Connect With Me

<p align="center">
  <a href="mailto:rohitrawat89199@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-FF6B6B?style=for-the-badge&logo=gmail&logoColor=white&labelColor=00000020" />
  </a>
  <a href="https://www.linkedin.com/in/rohit-rawat-7383091a7/">
    <img src="https://img.shields.io/badge/LinkedIn-58A6FF?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=00000020" />
  </a>
  <a href="https://github.com/RohitRawat891997">
    <img src="https://img.shields.io/badge/GitHub-1F2328?style=for-the-badge&logo=github&logoColor=white&labelColor=00000020" />
  </a>
  <a href="https://hub.docker.com/u/rohitrawat891997">
    <img src="https://img.shields.io/badge/DockerHub-2496ED?style=for-the-badge&logo=docker&logoColor=white&labelColor=00000020" />
  </a>
</p>
---

# 🐍 Python Notes — Identifiers, Type Casting & Conditional Statements

---

# 📌 Rules of Identifiers in Python

Identifiers are names given to:

* Variables → `x = 90`
* Functions → `def adduser():`
* Classes → `class Student:`

### ✅ Rules:

1. Can contain:

   * `a-z`
   * `A-Z`
   * `0-9`
   * `_` (underscore)

2. Must start with:

   * A letter (`a-z` or `A-Z`)
   * Or `_`

3. ❌ Cannot contain spaces

4. ❌ Cannot use Python keywords

Example:

```python
student_name = "Amit"
```

---

## 🔑 Python Keywords

```python
import keyword
print(keyword.kwlist)
```

Keywords are reserved words like:

```
False, None, True, and, as, assert, async, await,
break, class, continue, def, del, elif, else,
except, finally, for, from, global, if, import,
in, is, lambda, nonlocal, not, or, pass, raise,
return, try, while, with, yield
```

You cannot use them as variable names.

---

# 🧠 `id()` Function

```python
help(id)
```

### Purpose:

Returns the unique identity of an object (memory address in CPython).

```python
x = 90
print(id(x))
```

---

# 🔁 Loop Example

```python
row1 = [101, "Amit", 23, "Delhi"]

for x in row1:
    print(x, end=" ")
```

Output:

```
101 Amit 23 Delhi
```

---

# 🖨️ `print()` Advanced Usage

### Using `sep`

```python
x = "Amit"
y = "Kumar"
z = 101

print(x, y, z, sep=";")
```

Output:

```
Amit;Kumar;101
```

---

# ⌨️ Input Function

```python
x = input("Enter a number :")
y = input("Enter a number :")

z = x + y
print(z)
```

Output:

```
2
3
23
```

⚠️ Reason: `input()` always returns **string**

```python
print(type(x))  # <class 'str'>
```

---

# 🔄 Type Casting

Type casting converts one data type into another.

---

## 📂 File Reading Returns String

```python
data = open("abc.txt").read()
print(type(data))  # str
```

---

# 🧮 Type Conversion Functions

## 1️⃣ `int(x)`

| Example     | Result  |
| ----------- | ------- |
| `int(23.8)` | 23      |
| `int(True)` | 1       |
| `int('23')` | 23      |
| `int(3+5j)` | ❌ Error |

---

## 2️⃣ `float(x)`

| Example         | Result  |
| --------------- | ------- |
| `float(34)`     | 34.0    |
| `float(True)`   | 1.0     |
| `float("34.5")` | 34.5    |
| `float(4+5j)`   | ❌ Error |

---

## 3️⃣ `bool(x)`

Returns `False` when value is:

* `0`
* `0.0`
* `""`
* `0+0j`

Otherwise returns `True`.

---

## 4️⃣ `str(x)`

Converts value into string.

---

## 5️⃣ `complex()`

```python
complex(23)       # 23+0j
complex(23, 9)    # 23+9j
```

---

# 🧮 Correct Way to Add User Input

```python
x = int(input("Enter a number :"))
y = int(input("Enter a number :"))

z = x + y
print(z)
```

---

# 🔀 Conditional Statements

---

## Basic `if`

```python
if 40 > 5:
    print("line1")
    print("line2")
```

---

## `if-else`

```python
age = int(input("Enter your age :"))

if age > 18:
    print("valid")
else:
    print("not valid")
```

---

## Comparing Two Numbers

```python
x = int(input("Enter a number :"))
y = int(input("Enter a number :"))

if x > y:
    print("x is greater")
else:
    print("y is greater")
```

---

## Nested `if`

```python
if x != y:
    if x > y:
        print("x is greater")
    else:
        print("y is greater")
else:
    print("both are equal")
```

---

## 🔐 Login Example

```python
user = input("Enter username :")
password = input("Enter password :")

if user == "admin" and password == "@123":
    print("Login Successful")
else:
    print("Login Fail")
```

---

# 💰 Discount Logic Example

## Basic Version

```python
day = input("Enter day :")
amount = int(input("Enter amount :"))

if day.lower() == "sunday" and amount >= 5000:
    discount = (amount * 10) / 100
    amount = amount - discount
    print("After 10% discount price will be :", amount)
else:
    print("without discount price will be :", amount)
```

---

## Using `elif`

```python
if day.lower() == "sunday" and amount >= 5000:
    discount = (amount * 10) / 100
elif day.lower() == "sunday" and amount >= 4000:
    discount = (amount * 5) / 100
elif day.lower() == "sunday" and amount >= 3000:
    discount = (amount * 2) / 100
else:
    discount = 0

amount = amount - discount
print("Final price :", amount)
```

---

## Using List Membership

```python
if day.lower() in ["sunday", "saturday"] and amount >= 5000:
```

---

## Nested Discount Logic

```python
if day.lower() == "sunday":
    if amount >= 5000:
        discount = (amount * 10) / 100
        amount -= discount
        print("After discount :", amount)
    else:
        print("without discount :", amount)
else:
    print("without discount :", amount)
```

---

# 👨‍💻 Author

**Name:** Rohit Rawat<br>
**GitHub:** [https://github.com/RohitRawat891997](https://github.com/RohitRawat891997)<br>
**LinkedIn:** [https://www.linkedin.com/in/rohit-rawat-7383091a7/](https://www.linkedin.com/in/rohit-rawat-7383091a7/)

---

