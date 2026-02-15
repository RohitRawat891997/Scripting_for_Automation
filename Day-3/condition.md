# 🔀 Shell Scripting – Conditional Statements (if / test)

Conditional statements are used to **check whether a condition is true or false** and then execute commands based on the result.

In shell scripting, we commonly use:

* `if`
* `test`
* `[ condition ]`

---

## ❓ What is a Conditional Statement?

A conditional statement helps the script make decisions.

👉 It checks a condition and runs commands only if the condition is satisfied.

Example idea:

* If number is less than 10 → print message.
* If file exists → perform action.

---

## 🧪 How Conditions Are Tested in Shell

We usually use the `test` command or square brackets `[ ]`.

All of these are valid:

```bash
test expression
[ expression ]
if test condition
if [ condition ]
```

---

### ✅ Examples

```bash
if [ $i -lt 10 ]
if test $i -lt 10
if [ $? -eq 0 ]
if test $? -eq 0
```

---

## 📌 Types of `if` Syntax in Shell

There are mainly 3 types of conditional structures:

---

## 1️⃣ Simple `if ... fi`

Used when only **one condition** needs to be checked.

### Syntax:

```bash
if [ condition ]
then
    commands
fi
```

⚠️ `{ }` braces are optional.

---

### Example:

```bash
#!/bin/bash

i=5

if [ $i -lt 10 ]
then
    echo "Value is less than 10"
fi
```

---

## 2️⃣ `if ... else ... fi`

Used when you want two outcomes:

* One if condition is true
* Another if condition is false

### Syntax:

```bash
if [ condition ]
then
    commands
else
    commands
fi
```

---

### Example:

```bash
#!/bin/bash

num=15

if [ $num -lt 10 ]
then
    echo "Number is small"
else
    echo "Number is greater than or equal to 10"
fi
```

---

## 3️⃣ Nested / Multiple Conditions (`elif`)

Used when checking multiple conditions.

### Syntax:

```bash
if [ condition-1 ]
then
    commands
elif [ condition-2 ]
then
    commands
elif [ condition-3 ]
then
    commands
else
    commands
fi
```

---

### Example:

```bash
#!/bin/bash

marks=75

if [ $marks -ge 90 ]
then
    echo "Grade A"
elif [ $marks -ge 75 ]
then
    echo "Grade B"
elif [ $marks -ge 60 ]
then
    echo "Grade C"
else
    echo "Fail"
fi
```

---

## ⚠️ Important Note

We cannot use `if` without a test condition.

Valid formats:

```bash
if [ condition ]
if test condition
```

Examples:

```bash
if [ $i -lt 10 ]
if test $i -lt 10
```

---

## 🧩 Types of Testing Operators

There are four main types of comparison operators in shell scripting.

---

### 1️⃣ Numeric Testing Operators

Used for numbers.

| Operator | Meaning          |
| -------- | ---------------- |
| `-eq`    | equal            |
| `-ne`    | not equal        |
| `-gt`    | greater than     |
| `-lt`    | less than        |
| `-ge`    | greater or equal |
| `-le`    | less or equal    |

Example:

```bash
if [ $a -gt $b ]
then
    echo "a is greater"
fi
```

---

### 2️⃣ String Testing Operators

Used for text comparison.

| Operator | Meaning          |
| -------- | ---------------- |
| `=`      | equal            |
| `!=`     | not equal        |
| `-z`     | empty string     |
| `-n`     | non-empty string |

Example:

```bash
name="Rohit"

if [ "$name" = "Rohit" ]
then
    echo "Name matched"
fi
```

---

### 3️⃣ File Testing Operators

Used to check file properties.

| Operator | Meaning          |
| -------- | ---------------- |
| `-f`     | file exists      |
| `-d`     | directory exists |
| `-r`     | readable         |
| `-w`     | writable         |
| `-x`     | executable       |

Example:

```bash
if [ -f "test.txt" ]
then
    echo "File exists"
fi
```

---

### 4️⃣ Logical / Boolean Operators

Used to combine conditions.

| Operator | Meaning |   |    |
| -------- | ------- | - | -- |
| `&&`     | AND     |   |    |
| `||`     | OR      | ` |    |
| `!`      | NOT     |   |    |

Example:

```bash
if [ $a -gt 5 ] && [ $b -lt 10 ]
then
    echo "Both conditions true"
fi
```

---

## 📌 Summary

* Conditional statements help scripts make decisions.
* `if`, `test`, and `[ ]` are used to check conditions.
* Types of conditions include numeric, string, file, and logical operators.
* Multiple conditions can be handled using `elif`.

---
