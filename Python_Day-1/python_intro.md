[![LinkedIn](https://img.shields.io/badge/Connect%20with%20me%20on-LinkedIn-blue.svg)](https://www.linkedin.com/in/rohit-rawat-7383091a7/)
[![GitHub](https://img.shields.io/github/stars/AmanPathak-DevOps.svg?style=social)](http://github.com/RohitRawat891997)
[![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)](https://app.docker.com/accounts/rohitrawat891997)

# 🐍 Python Basics — Day 1 Notes
---

## 📌 What is Python?

**Python** is a **high-level, general-purpose programming language** that is easy to read and write. It is widely used in automation, DevOps, web development, AI, and scripting.

---

## 🕰️ Python History

* **1989 – 1991** → Created by *Guido van Rossum*
* **Python 1.x** → Released in 1994
* **Python 2.x** → Released in 2000

```python
print "Hello"
```

* **Python 3.x** → Released in 2008

```python
print("Hello")
```

### 🔧 Tool used for conversion from Python 2 to Python 3

The primary and official tool for converting code from Python 2 to Python 3 is **`2to3`**.

It is a Python program that reads Python 2.x source code and applies a series of "fixers" to transform it into valid Python 3.x code. While `2to3` is the standard, there are several other tools often preferred depending on whether you need to maintain backward compatibility with Python 2.

---

### 1️⃣ The Official Tool: `2to3`

This tool is usually installed with the Python interpreter. It performs a **one-way conversion**, meaning the output is intended to run **only** on Python 3.

**How to use it:**

```bash
# To see a diff of changes without applying them
2to3 my_script.py

# To apply the changes and overwrite the file (creates a backup)
2to3 -w my_script.py
```

**Best for:** Projects that are moving entirely to Python 3 and will never look back.

---

### 2️⃣ Modern Alternatives

Many developers prefer these tools because they help create cleaner code or allow the same codebase to run on **both Python 2 and 3**.

| Tool               | Purpose                                           | Key Feature                                           |
| ------------------ | ------------------------------------------------- | ----------------------------------------------------- |
| `python-modernize` | Transition to Py3 while keeping Py2 compatibility | Uses the `six` library                                |
| `futurize`         | Part of python-future library                     | Makes Py2 code look like clean Py3                    |
| `pyupgrade`        | Modernizes syntax for newer Py3 versions          | Converts old syntax to modern features like f-strings |

---

### 3️⃣ Key Manual Considerations

Even the best tools cannot fix everything. You may need to manually handle:

* **Strings vs Bytes** → Python 3 is stricter about text vs binary
* **Dictionary methods** → `d.iteritems()` → `d.items()`
* **Division behavior** → `1/2` = `0.5` in Py3 but `0` in Py2

> 💡 **Pro Tip:** Always run your unit tests before and after conversion to ensure nothing breaks.

---

## ⭐ Features of Python

### ✅ Simple

Python syntax is easy and beginner-friendly.

### ✅ Platform Independent

Runs on Windows, Linux, and macOS.

### ✅ Open Source

Free to use with a strong community.

### ✅ Dynamic Language

No need to declare data types explicitly.

---

## ⚙️ Static vs Dynamic Typing

### 🔵 Static Typing (C, C++)

```c
int age = 90;
```

### 🟢 Dynamic Typing (Python)

```python
age = 90
```

---

## 📊 Example Data in Python

```python
id = 101
name = "Amit"
age = 45.6
city = "Delhi"
```

Python automatically detects variable types at runtime.

---

## 🧠 Interpreter Language

Python is an **interpreted language**, meaning code runs **line by line**.

```python
print("hello1")
print("hello2")
print("hello3")
```

---

# 📝 Day-1 Assignment

👉 Write a Python program to print your name 10 times.

### ✅ Example Solution

```python
for i in range(10):
    print("Rohit Rawat")
```

---

# 👨‍💻 Author

**Name:** Rohit Rawat<br>
**GitHub:** https://github.com/RohitRawat891997<br>
**LinkedIn:** https://www.linkedin.com/in/rohit-rawat-7383091a7/


---
