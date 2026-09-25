# 🏦 Bank Account Management System

A beginner-friendly **Python Bank Account Management System** built as part of my Bleep India programming project series.

The project allows users to create bank accounts, deposit and withdraw money, check account balances, and view transaction history. Account records are stored persistently in a **JSON file**, so the data can be loaded again when the notebook is reopened.

---

## 📌 Project Overview

The objective of this project is to build a simple banking system using core Python concepts such as:

- Lists and dictionaries
- Functions
- Loops and conditional statements
- User input
- File handling
- JSON data storage
- Date and time handling
- Transaction history
- Menu-driven programming

The project is implemented in a **Jupyter Notebook** and uses `bank.json` for persistent data storage.

---

## ✨ Features

### 1. Create Account

Users can create a new bank account by entering:

- Account number
- Account holder's name
- Initial deposit

The system also checks whether the account number already exists before creating a new account.

### 2. Deposit Money

Users can deposit money into an existing account.

The system:

- Finds the account using the account number
- Adds the deposit amount to the current balance
- Creates a transaction record
- Stores the transaction date and time
- Saves the updated records to `bank.json`

### 3. Withdraw Money

Users can withdraw money from an existing account.

The system:

- Finds the account
- Checks whether sufficient balance is available
- Deducts the withdrawal amount
- Creates a withdrawal transaction record
- Stores the transaction date and time
- Saves the updated records

If the requested withdrawal is greater than the available balance, the system displays:

`Insufficient balance!`

### 4. Check Balance

Users can enter an account number to view:

- Account holder's name
- Current account balance

### 5. Transaction History

Users can view the transaction history of an account.

Each transaction displays:

- Transaction type
- Amount
- Date and time

If an account has no transactions, the system displays:

`No transactions found!`

### 6. Persistent Data Storage

The project uses a JSON file named:

`bank.json`

The `save_records()` function writes the current account data to the JSON file.

When the notebook starts, the existing data is loaded from the same file. If the file does not exist, an empty list is created.

---

## 🛠️ Technologies Used

- **Python**
- **Jupyter Notebook**
- **JSON**
- **Python `datetime` module**

### Python Modules

```python
import json
from datetime import datetime

Author Shriya Verma
Data Analytics August Batch 
