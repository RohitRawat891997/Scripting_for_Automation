#Bash Scripting
---

# 🐚 Shell Scripting Notes

This repository contains beginner-friendly notes about **Shell**, **Shell Scripting**, **Kernel**, and **Variables** in Linux.
These notes are written in a simple way to help understand basic Linux scripting concepts.

---

## 📜 What is a Script?

A **script** or **scripting language** is a programming language used in a special run-time environment to automate tasks.

Instead of running commands manually one by one in the CLI, scripts allow automation of repetitive work.

---

## ⚙️ What is Shell Scripting?

A **Shell Script** is a computer program designed to run inside the Unix/Linux shell.

👉 Key Points:

* A shell script is a series of commands written in a plain text file.
* Similar to a **batch file** in MS-DOS.
* Used to automate Linux command-line tasks.

---

## ❓ Why Do We Use Shell Scripting?

Shell scripting helps in automation and reduces manual work.

### Benefits:

1. Prepare input files, job monitoring, and output processing.
2. Create custom commands.
3. Save time in file processing.
4. Automate daily tasks.
5. Automate system administration activities.
6. Perform backups and monitoring.
7. Reduce admin workload.
8. Manage multiple servers from one place.
9. Work smarter with automation.

---

## 🖥️ What is a Shell?

The **Shell** is an interface between the **user** and the **Linux kernel**.

👉 How it works:

* Accepts user commands (mostly in English).
* Validates the command.
* Passes it to the kernel for execution.

---

## 🧩 Types of Supported Shells in Linux

| Shell Name                | Command Path |
| ------------------------- | ------------ |
| Bourne Shell              | `/bin/sh`    |
| Bourne Again Shell (Bash) | `/bin/bash`  |
| Korn Shell                | `/bin/ksh`   |
| C Shell                   | `/bin/csh`   |
| Turbo C Shell             | `/bin/tcsh`  |

---

## ❤️ What is Kernel?

The **Kernel** is the heart of the Linux Operating System.

👉 Responsibilities:

* Acts as an interface between hardware and software.
* Manages system resources.
* Controls execution of programs.
* Communicates between shell, applications, and hardware.

---

## 🧠 What Does the Kernel Do?

### Core Functions:

* Memory Management
  ➝ Tracks memory usage and allocation.

* Process Management
  ➝ Decides which process uses CPU and for how long.

* Device Drivers
  ➝ Communicates between hardware and processes.

* System Calls & Security
  ➝ Handles service requests from applications.

### Resource Management Includes:

* I/O Management
* Process Management
* Device Management
* File Management
* Memory Management

---

## 🔍 How to Check Kernel Version?

Run the following commands:

```bash
uname
uname -r
ls /boot
```

---

## 🔢 Variables in Shell

Variables are symbolic names that store values in memory.

### Types of Variables in Linux Shell

---

### 1️⃣ System Defined Variables (SDV)

* Created and maintained by Linux.
* Usually written in **CAPITAL LETTERS**.

Example:

```bash
echo $HOME
echo $PATH
```

---

### 2️⃣ User Defined Variables (UDV)

* Created and managed by users.
* Usually written in **lowercase**.

Example:

```bash
name="Rohit"
echo $name
```

---

## 📌 Summary

* Shell scripting automates repetitive Linux tasks.
* The shell acts as a bridge between user and kernel.
* The kernel manages hardware resources and processes.
* Variables help store and manage data inside scripts.

---

