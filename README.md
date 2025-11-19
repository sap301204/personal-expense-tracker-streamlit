# Personal Expense Tracker with Data Visualization (Python + Streamlit + SQLite)

This is an industry-ready, end-to-end Personal Expense Tracker project built using Python, Streamlit, SQLite, Pandas, and Matplotlib.  
It allows users to upload bank/UPI CSV files, automatically categorizes expenses, visualizes spending patterns, tracks budgets, and exports monthly Excel reports.

---

## 🚀 Features
- 🔄 CSV ingestion (UPI / Bank statements / Custom CSV)
- 🧠 Auto-categorization using rule-based classifier
- 🗄️ SQLite backend (portable database)
- 📊 Interactive Streamlit dashboard 
- 📉 Monthly spend trend + category donut + merchant bar chart
- 📈 KPIs: Total Spend, Income, Savings
- 💰 Budgeting system with overspend alerts
- 📤 Export monthly Excel report (XLSX)
- 🧱 Clean folder structure with modular Python code

---

## 🗂️ Project Structure


expense-tracker/
├── src/
│ ├── models.py
│ ├── ingest.py
│ ├── categorize.py
│ ├── analyze.py
│ ├── plots.py
│ ├── budget.py
│ └── app_streamlit.py
├── data/
│ └── sample_transactions.csv
├── db/
├── exports/
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore


---

## 📦 Installation & Setup

### 1️⃣ Create Virtual Environment


python -m venv venv


### 2️⃣ Activate  
**Windows**


venv\Scripts\activate

**Mac/Linux**


source venv/bin/activate


### 3️⃣ Install Dependencies


pip install -r requirements.txt


### 4️⃣ Initialize Database


python -c "from src.models import init_db; init_db()"


### 5️⃣ Run Streamlit App


streamlit run src/app_streamlit.py


---

## 📥 How to Add Transactions
Upload any CSV (bank/UPI/exported statements) through the Streamlit sidebar.  
The app auto-detects columns & normalizes them.

---

## 📊 Example Visualizations
- Monthly Spend Trend  
- Category Donut Chart  
- Top Merchants Bar Chart  
- KPI Cards  

*(Screenshots can be placed in `assets/screenshots/`)*

---

## 📤 Export Monthly Report


from src.report import export_month
export_month("2025-11")


---

## 📜 License
This project is licensed under the MIT License.

---

## 🤝 Contribute
Feel free to fork, improve modules, or add ML categorization!

---

## ⭐ Support
If this project helps you, please ⭐ star the repo!

