# 💰 Expense Tracker

A simple, elegant **Expense Tracker** built with **HTML, CSS, and JavaScript**.  
It helps you keep track of your **income** and **expenses**, shows your **balance**, and stores all transactions using **localStorage** so your data is saved even after refreshing the page.

---

## 🚀 Features
- ✅ Add income & expenses
- ✅ Display total **balance, income, and expenses**
- ✅ Delete transactions
- ✅ Persist data using **localStorage** (stays even after refresh)
- ✅ Responsive design (works on mobile & desktop)
- ✅ Smooth animations and modern UI

---

## 📂 Project Structure
expense-tracker/
│── index.html # Structure of the app
│── style.css # Styling and layout
│── script.js # App logic (transactions, storage, calculations)


---

## 🖥️ How It Works
1. Enter a **description** (e.g., "Salary" or "Groceries").  
2. Enter an **amount**:
   - Positive (`+1000`) → Income 💵  
   - Negative (`-200`) → Expense 💸  
3. Click **Add Transaction**.  
4. The transaction appears in the list and updates:
   - ✅ Balance  
   - ✅ Income total  
   - ✅ Expenses total  
5. Transactions are saved in **localStorage**.  
6. You can remove a transaction by clicking the **❌ button**.

---

## 🛠️ Technologies Used
- **HTML5** → Structure
- **CSS3** → Styling and responsiveness
- **JavaScript (ES6)** → Logic, DOM manipulation, localStorage

---

## 📜 Code Overview

### 🔹 HTML (`index.html`)
- Contains:
  - **Balance section**
  - **Income & Expense summary**
  - **Transaction list**
  - **Form to add transactions**

### 🔹 CSS (`style.css`)
- Clean, modern design with gradients  
- Styled **transaction list** with hover animations  
- **Responsive layout** for mobile users  

### 🔹 JavaScript (`script.js`)
- Stores transactions in an array:
  ```js
  let transactions = JSON.parse(localStorage.getItem("transactions")) || [];

Functions:
  -  addTransaction() → Adds a new transaction
  -  updateTransactionList() → Updates the list on screen
  -  updateSummary() → Updates balance, income, expenses
  -  removeTransaction(id) → Deletes a transaction
  -  formatCurrency() → Formats numbers into $ currency

## 1. Clone or download this repository:
    git clone https://github.com/your-username/expense-tracker.git
## 2. Open the folder:
    cd expense-tracker
## 3. Open index.html in your browser


## 📌 Future Improvements:
- Add categories (Food, Rent, Shopping, etc.)
- Show charts/graphs using Chart.js
- Add dark mode toggle
- Export transactions to CSV/PDF