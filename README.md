# Spending Management App

This is a simple desktop application for managing and tracking personal spending, built with Python. The application uses `tkinter` and `customtkinter` for the user interface and `SQLite` for data storage.

## Key Features

The application is divided into two main tabs: "Dashboard" and "Summary".

### 1. Dashboard

This is where you enter and manage your daily transactions.

* **Expense Tracking:**
    * **Add:** Record new expenses including Category, Item Name, Price, and Date.
    * **Update:** Edit previously entered expense records.
    * **Delete:** Remove expenses from the database.
    * **Display:** All expenses are clearly displayed in a table.
* **Income Tracking:**
    * **Add:** Record income (e.g., Salary, Gifts, etc.).
    * **Update & Delete:** Manage income records similarly to expenses.
    * **Display:** A separate table for income records.
* **Total Balance:**
    * A display for the **Total Balance** is automatically calculated (Total Income - Total Expense) and updates in real-time.
* **Utilities:**
    * "Current Date" button to automatically fill in the current date.
    * "Clear Entry" button to quickly clear input fields.
    * Date validation (DD/MM/YYYY) to ensure data accuracy.

### 2. Summary

This tab provides a visual overview of your financial situation through charts (using Matplotlib).

* **Summary by Days:** A bar chart comparing total income and expenses for the **last 7 days**.
* **Summary by Months:** A bar chart summarizing income/expenses for the **12 months of the current year**.
* **Summary by Years:** A bar chart summarizing income/expenses for the **last 4 years**.
* **Pie Chart:** A pie chart showing the percentage breakdown of income and expense categories for the **current month**.

## Technology Stack

* **Language:** Python 3
* **GUI:** `tkinter` and `customtkinter`
* **Data Viz:** `matplotlib`
* **Data Processing:** `pandas` and `numpy`
* **Database:** `sqlite3` (via the custom `Database` class in `mydb.py`)
* **Other:** `Pillow (PIL)` (for icon image handling)
