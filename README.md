# Python Text Calculator 🧮

A simple text-based calculator that processes mathematical and logical operations from input files and outputs results to text files.

## 📋 Project Overview

This Python program reads a text file containing lines of mathematical and logical operations, evaluates them according to Python operator precedence, and writes the results to an output file. Invalid operations are handled with appropriate error messages.

## ✨ Features

- 📁 **File-based input/output processing**
- 🔢 **Arithmetic operations**: `**`, `*`, `//`, `/`, `%`, `+`, `-`
- 🔍 **Logical operations**: `<`, `>`, `==`, `!=`
- 📐 **Multiple operations per line** with proper precedence
- ⚠️ **Comprehensive error handling**
- 📝 **Empty line preservation**
- 🎯 **Space-insensitive parsing**

## 🎮 How It Works

### **Input Processing:**
- Reads `input.txt` line by line
- Parses mathematical expressions
- Handles both spaced and non-spaced formats
- Validates syntax and operands

### **Operation Support:**
Arithmetic:     3 + 4, 5 ** 2, 7 // 2, 11 % 3
Logical:        5 > 3, 4 == 4, 3 != 5
Multiple:       2 + 3 * 4 (follows Python precedence)

### **Error Handling:**
- Invalid characters → `ERROR`
- Missing operands → `ERROR`
- Division by zero → `ERROR`
- Malformed expressions → `ERROR`

## 🚀 How to Run

```bash
# Run the calculator
python 2021510062_irem_tekin.py

# Make sure you have:
# - input.txt in the same directory
# - Write permissions for output file
📄 File Format
Input File (input.txt):
3 + 4
5**2
7 // 2
5 > 3
3 == 5

2 + 3 * 4
invalid + expression
Output File (*_output.txt):
7
25
3
True
False

14
ERROR
📊 Supported Operations
OperationSymbolExampleResultPower**5 ** 225Multiplication*3 * 412Integer Division//7 // 23Division/5 / 22.5Modulus%7 % 31Addition+3 + 47Subtraction-5 - 23Less Than<3 < 5TrueGreater Than>5 > 3TrueEqual==4 == 4TrueNot Equal!=3 != 5True
🔧 Technical Details
Operator Precedence:
Follows Python's operator precedence rules:

** (Power)
*, /, //, % (Multiplication, Division)
+, - (Addition, Subtraction)
<, >, ==, != (Comparison)

Algorithm:

Tokenization: Split expressions into numbers and operators
Validation: Check for valid syntax and operands
Evaluation: Process operations according to precedence
Output: Write results or ERROR messages

Error Cases:

Non-numeric characters (except operators)
Missing operands
Division by zero
Invalid operator combinations
Malformed expressions

💡 Example Usage
Complex Expressions:
Input:  2 + 3 * 4
Output: 14         (follows precedence: 3*4=12, 2+12=14)

Input:  2 * 3 + 4
Output: 10         (follows precedence: 2*3=6, 6+4=10)

Input:  10 / 2 == 5
Output: True       (10/2=5.0, 5.0==5 is True)
🎯 Learning Objectives
This project demonstrates:

File I/O operations in Python
String processing and parsing
Mathematical expression evaluation
Operator precedence implementation
Comprehensive error handling
Recursive algorithm design

👨‍💻 Author
İrem TEKİN
Computer Engineering Student - Dokuz Eylül University
📧 [iremtekin1107@gmail.com]
🔗 [https://www.linkedin.com/in/irem-tekin11/]
📜 Academic Note
This project was created for educational purposes as part of CME1203 Introduction to Computer Engineering course, focusing on file processing and mathematical expression evaluation in Python.

⭐ Don't forget to star this repository if you found it helpful!
