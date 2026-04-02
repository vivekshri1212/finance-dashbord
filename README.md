# 💹 FinanceIQ — Finance Dashboard UI

A clean and interactive **Finance Dashboard** built with plain **HTML, CSS, and JavaScript**.  
This project was built as part of a Frontend Developer Intern assignment.

---

## 🚀 How to Run

No installation required. No framework. No build step.

1. Download the `finance-dashboard.html` file
2. Open it in any browser (Chrome, Firefox, Edge)
3. That's it — the dashboard will load instantly ✅

---

## 📁 Project Structure

```
finance-dashboard.html   ← Single file containing HTML + CSS + JavaScript
README.md                ← This file
```

---

## ✨ Features

### 1. 📊 Dashboard Overview
- **Summary Cards** — Total Balance, Total Income, Total Expenses
- **Line Chart** — Monthly balance trend (Oct to Mar)
- **Doughnut Chart** — Spending breakdown by category
- **Recent Transactions** — Last 5 transactions at a glance

### 2. 💳 Transactions Section
- Full list of all transactions with Date, Description, Category, Type, and Amount
- **Search** — Search by description or category
- **Filter** — Filter by type (Income/Expense) and category
- **Sort** — Sort by newest, oldest, highest or lowest amount
- **Add Transaction** — Admin can add new transactions via modal form
- **Edit Transaction** — Admin can edit any existing transaction
- **Delete Transaction** — Admin can delete transactions with confirmation

### 3. 🔐 Role Based UI
- **Admin Role** — Can add, edit, and delete transactions
- **Viewer Role** — Can only view data, no edit access
- Switch roles using the dropdown in the top navigation bar
- UI updates automatically based on selected role

### 4. 📈 Insights Section
- **Highest Spending Category** — Shows which category has most expenses with visual bars
- **Monthly Comparison** — February vs March expense and income comparison
- **Savings Rate** — Percentage of income saved with progress bar
- **Observations** — Auto-generated smart insights based on the data

### 5. 🎨 UI/UX
- Dark theme with clean modern design
- Smooth animations and hover effects
- Fully **responsive** — works on mobile, tablet, and desktop
- Empty state handling when no transactions found

---

## 🛠️ Tech Stack

| Technology | Usage |
|---|---|
| HTML5 | Structure and layout |
| CSS3 | Styling, animations, responsive design |
| JavaScript (ES6+) | Logic, state management, DOM manipulation |
| Chart.js (CDN) | Line chart and Doughnut chart |
| Google Fonts | DM Serif Display + DM Sans typography |

---

## 📦 State Management

All application state is managed using plain JavaScript variables:

- `transactions` — Array storing all transaction data
- `role` — Stores current user role (admin/viewer)
- `editId` — Tracks which transaction is being edited

State updates trigger UI re-renders via dedicated render functions:
- `renderDashboard()` — Updates cards, charts, recent table
- `renderTransactions()` — Updates full transaction table with filters
- `renderInsights()` — Updates all insight sections

---

## 🔍 Assumptions Made

- Data is static/mock — no backend or database connected
- Transactions are pre-loaded with sample data for demonstration
- Role switching is done via dropdown for demo purposes
- Charts use CDN version of Chart.js (internet connection needed for charts)

---

## 📱 Responsive Behavior

| Screen Size | Layout |
|---|---|
| Desktop (>900px) | Sidebar + full layout |
| Tablet (600–900px) | No sidebar, 2-column cards |
| Mobile (<600px) | Single column, compact controls |

---

## 👨‍💻 Developer

**Vivek Kumar**  
Frontend Developer Intern  
B.Tech Computer Science Engineering — IITM Group of Institutions (2022–2026)  
GitHub: [github.com/vivekshri1212](https://github.com/vivekshri1212)  
Email: shrivastavvivek713@gmail.com

---

## 📝 Notes

- This project focuses on UI design, component structure, and frontend logic
- It is not production-ready and does not require any backend
- All data resets on page refresh (no localStorage used)
