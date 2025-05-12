# Google Sheets Expense Tracker 💰📊

## 🚀 Project Description

This project allows you to track your daily and other expenses using Google Sheets. It helps you monitor your budgets for different categories like **Daily Foods** 🍽️ and **Other Expenses** 💵 while automatically updating the total amount and remaining budget in real-time.

With automatic date and time stamps, the tracker helps you visualize your spending and manage your finances more effectively. Whether you're tracking a small grocery budget or large monthly expenses, this tool will keep you on track!

## 🛠 Features

* **Automatic Setup:** Automatically creates and sets up the necessary sheets: "Daily Foods" and "Other Expenses" 📑.
* **Real-Time Updates:** When a new expense is added, the date, time, and updated amounts are automatically recorded 🕒.
* **Budget Tracking:** Each sheet has its own budget (Daily Foods with ₹3000, Other Expenses with ₹7000), and remaining budgets are calculated automatically 📉.
* **Total Expense Log:** All expenses are logged in the "Total Amount" sheet, including the updated remaining balance 💸.
* **Expense Deletion Handling:** If an expense is removed, the corresponding data is updated to reflect the change 📂.

## 📊 Setup Instructions

### 1. Create a New Google Sheets File

* Open [Google Sheets](https://sheets.google.com).
* Create a new spreadsheet.

### 2. Add the Script

* In the Google Sheets document, go to **Extensions > Apps Script**.
* Delete any existing code and paste the provided script into the editor.
* Save and run the script.

### 3. Track Your Expenses

* After running the script, two sheets will be created: "Daily Foods" and "Other Expenses."
* Add your expenses under the "Price" column, and the date and time will be automatically updated.
* View the "Total Amount" sheet for a summary of all expenses and remaining balances.

## 🎯 Usage Example

* **Daily Foods:** Track your daily meals and snacks 🍲.
* **Other Expenses:** Track everything else like shopping, bills, etc. 🛒.
* **Total Amount:** View your total expenses and remaining budget in real-time 📈.

## 📈 Budget Setup

* **Daily Foods:** ₹3000 max budget 💸
* **Other Expenses:** ₹7000 max budget 🏷️
* **Total Amount:** ₹55855 initial amount for logging all expenses 💰

## ⚙️ How It Works

The script will:

1. **Create Sheets:** Automatically creates "Daily Foods" and "Other Expenses" sheets.
2. **Setup Columns:** Sets up columns for date, time, description, and price of each expense.
3. **Track Expenses:** Every time you add an expense, the script logs the expense in the "Total Amount" sheet.
4. **Update Budgets:** Each expense is deducted from the allocated budget, and remaining amounts are updated in real-time.

## 👨‍💻 Code Overview

* **setupExpenseSheets():** Initializes the expense sheets and sets up the budgets.
* **setupSheet(sheet, maxBudget):** Configures each sheet (Daily Foods, Other Expenses) with headers, column widths, and formulas.
* **setupTotalAmountSheet():** Sets up the "Total Amount" sheet for tracking all expenses.
* **onEdit(e):** Triggers when an edit is made to update the date/time and log the expense.
* **logExpenseToTotalAmount():** Adds an expense to the "Total Amount" sheet and updates the remaining balance.
* **removeExpenseFromTotalAmount(row):** Removes an expense when deleted and updates the remaining amount.

## 📅 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
