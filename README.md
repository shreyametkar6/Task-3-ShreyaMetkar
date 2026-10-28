# Task 3: Random Password Generator (Python)

## Description
A command-line password generator written in Python. The user enters a password length, and the program generates a random, secure password using letters and numbers (special characters are optional). It also shows the password's entropy in bits and a strength rating.

Built as **Task 3** of my Python Programming Internship at **DecodeLabs** (Batch 2026).

## Features
- Choose a password length from 8 to 128 characters
- Input validation (text and out-of-range numbers are rejected)
- Optional special characters (`@`, `#`, `$`, ...)
- Every password has at least one letter and one number
- Shows entropy in bits and a strength rating
- Tip based on the NIST 2024 guideline (15+ characters)

## How to Run
1. Install Python and Jupyter Notebook.
2. Download this repository (green **Code** button, then **Download ZIP**) and extract it.
3. Open a terminal in the extracted folder and start Jupyter:

```
jupyter notebook
```

4. Open `random_pwd_generator.ipynb`.
5. Click the code cell and press **Shift + Enter** to run it.
6. Enter a length, choose whether to include special characters, and read the result.

## Example
```
===== RANDOM PASSWORD GENERATOR =====
Enter password length (8-128): 20
Include special characters (@, #, $ ...)? (y/n): n

=============================
Password  : QXlPu6AEjupfwxscj5Gp
Length    : 20
Pool size : 62 characters
Entropy   : 119.1 bits (Very strong)
=============================
```

## Concepts Used
- Importing modules (`secrets`, `string`, `math`)
- `secrets.choice()` for cryptographically secure randomness
- `string.ascii_letters`, `string.digits`, `string.punctuation`
- `''.join()` instead of `password += char` (faster string building)
- Input validation with `try / except ValueError`
- Entropy formula: `E = L × log2(R)`

## Author
Shreya Metkar - [GitHub](https://github.com/shreyametkar6)
