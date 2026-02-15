# 🐚 Shell Scripting – Variables, Read, Expr & Exit Status Notes

These notes explain important shell scripting concepts like **variables**, **expr command**, **read command**, **quotes**, and **exit status** in a simple way.

---

## 🔢 Why Do We Use Variables in Linux?

Variables are used to store values that can be reused anywhere in a script.

### ✅ Benefits of Variables:

* Store user input or command output.
* Make scripts dynamic and reusable.
* Reduce repetition of values.
* Improve script readability.
* Help in automation and logic building.

---

## 🧩 Types of Variables in Linux

### 1️⃣ System Defined Variables (SDV)

* Created by the Linux system.
* Usually written in **CAPITAL LETTERS**.

Example:

```bash
echo $HOME
echo $USER
echo $PATH
```

---

### 2️⃣ User Defined Variables (UDV)

* Created by users inside scripts.
* Usually written in **lowercase**.

Example:

```bash
name="Rohit"
echo $name
```

---

## ➕ Expr Command

The `expr` command is used to perform **basic arithmetic operations** in shell scripting.

### Supported Operations:

* Addition
* Subtraction
* Multiplication
* Division
* Modulus

---

## 🧪 Examples of `expr` Command

```bash
expr 5 + 2
expr 10 - 3
expr 4 \* 3
expr 20 / 5
expr 10 % 3
```

⚠️ Note:

* Spaces are required between numbers and operators.
* Use `\*` for multiplication to avoid shell interpretation.

---

## ⌨️ Read Command

The `read` command is used to take **input from the keyboard** and store it in a variable.

👉 This variable can be used anywhere in the script.

### Syntax:

```bash
read variable_name
```

### Example:

```bash
echo "Enter your name:"
read name
echo "Hello $name"
```

---

## 📝 Types of Quotes in Shell

Quotes control how text and variables are interpreted.

---

### 1️⃣ Single Quotes `' '`

* Prints text **exactly as written**.
* Variables are NOT expanded.

Example:

```bash
echo 'Hello $USER'
```

Output:

```
Hello $USER
```

---

### 2️⃣ Double Quotes `" "`

* Used to print messages.
* Variables and special characters like `$` and `\` work inside double quotes.

Example:

```bash
echo "Hello $USER"
```

---

### 3️⃣ Back Quotes `` ` ` ``

* Used to execute commands and print their output.

Example:

```bash
`command`
```

OR modern syntax:

```bash
$(command)
```

Example:

```bash
echo "Today date is $(date)"
```

📌 Note:

* Double quotes `" "` can be used around back quotes.
* Single quotes `' '` cannot interpret command output.

---

## 🚦 Exit Status in Linux

Exit status shows whether the last command was executed successfully or not.

### How to Check Exit Status?

```bash
$?
```

### Meaning of Exit Codes:

* `0` ➝ Command executed successfully.
* `Non-zero` ➝ Error occurred.

Range:

```
0 – 255
```

### Example:

```bash
ls
echo $?
```

---

## 📌 Summary

* Variables store reusable values.
* `expr` performs arithmetic operations.
* `read` takes user input.
* Quotes control how text and variables behave.
* Exit status helps check command success or failure.

---

