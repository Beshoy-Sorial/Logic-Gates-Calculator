# ⚙️ Logic Gates Calculator (3-bit Signed Numbers)

## 📌 Overview

This project is a **Logic Gate-Based Calculator** capable of performing basic arithmetic operations — **Addition**, **Subtraction**, **Multiplication**, and **Modulus** — on **3-bit signed numbers**.

Each number is represented using **1 sign bit** and **2 bits for magnitude**, allowing signed values from **-3 to +3**. The calculator is built entirely using **primitive logic gates** (AND, OR, XOR, NOT) without using any high-level arithmetic operations.

---

## 🧠 Purpose

This project demonstrates how complex arithmetic operations can be constructed using only basic logic gates, similar to how real CPUs perform calculations at the hardware level.

---

## 🔢 Number Format

Each number is represented in **3 bits**:
- `[S][B1][B0]`
  - `S`: Sign bit (0 = positive, 1 = negative)
  - `B1B0`: 2-bit binary magnitude (00 = 0, ..., 11 = 3)

### Valid Range: `-3` to `+3`

| Decimal | 3-bit Binary |
|---------|--------------|
| -3      | 1 1 1        |
| -2      | 1 1 0        |
| -1      | 1 0 1        |
|  0      | 0 0 0        |
|  1      | 0 0 1        |
|  2      | 0 1 0        |
|  3      | 0 1 1        |

---

## 🧮 Supported Operations

All operations are manually implemented using **logic gate simulations**, such as half adders, full adders, multiplexer logic, and bitwise operations:

- ➕ **Addition (A + B)**
- ➖ **Subtraction (A - B)** (using two's complement)
- ✖️ **Multiplication (A × B)** (bit-shift and add logic)
- % **Modulus (A % B)** (subtractive method)

Each operation handles signed input and ensures output remains within 3-bit signed range, or it flags overflow.

---

## 🛠️ Built With

- 🧩 Basic logic gates (AND, OR, XOR, NOT)
- 🏗️ Composite gates (Half Adder, Full Adder, Two's Complement logic)

---
