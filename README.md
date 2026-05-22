# EduManage Pro - Enterprise Setup

**EduManage Pro** is an enterprise-grade academic and financial resource planning tool. It is engineered to securely manage student database records, visualize fiscal cash flow, track operational expenses, and leverage statistical machine learning to forecast academic performance.

---

## Architecture & Interface
Features a completely custom CSS layer built over Streamlit, enforcing a strict white-labeled, premium UI. The 'Carbon & Gold' theme utilizes a monochromatic dark carbon background with sophisticated amber/gold accents for a classic, high-finance aesthetic.

## Core System Modules
* **Centralized Admin Panel**: For system-wide statistics and master password management.
* **Secure Credential Storage**: The master password hash is stored securely in a local `auth.key` file, not hardcoded in the source.
* **Student Management**: Register students with parent details, class info, and track the date of their last payment.
* **AI-Powered Database Queries**: An integrated AI assistant (powered by Google Gemini) that converts natural language questions into SQL queries to analyze data.
* **Record Archiving**: Soft-delete functionality to archive past students instead of removing them permanently, preserving their historical data.
* **Financial Tracking**: Track 'Collected' revenue, 'Pending' payments, 'Business Expenses', and 'Net Profit' at a glance.
* **Academic Tracking**: Comprehensive module to mark daily attendance and log exam/test scores. 
* **Machine Learning Predictions**: Visually plots a student's performance trend line using NumPy Linear Regression and forecasts their next exam score.
* **Enterprise Security**: Master password is cryptographically protected using SHA-256 hashing.
* **Tutor Task Manager**: Integrated To-Do list to keep track of your daily educational tasks.
* **Global Search**: A unified search bar in the sidebar to instantly find records across students, expenses, and tasks.
* **Dynamic Search**: Instantly filter students by name.
* **Analytics**: Native Pandas-driven charts of revenue, cash flow, and class distributions, with an interactive raw data table.
* **Data Export**: Download your entire student database as a CSV with one click.
* **System Backup**: One-click export of the entire SQLite `.db` database file for secure data recovery and migration.
* **Edit Records**: Update student details seamlessly on the fly.
* **PDF Receipt Generation**: Download professional receipts for paid fees using `fpdf2`.
* **RDBMS Local Storage**: Zero-setup, optimized SQLite database engine.

## Technical Stack
* **Frontend**: Streamlit
* **Backend/Database**: SQLite + Pandas + NumPy (Machine Learning)
* **Architecture**: Single-Administrator with Secure File-Based Authentication
* **AI Integration**: Google Generative AI (Gemini)
* **Security**: Python `hashlib` (SHA-256)
* **Environment Management**: Python `uv`

## Deployment Setup
1. Clone the repo: `git clone https://github.com/AkshayaSanga/StudentManager.git`
2. Install dependencies: `uv pip install -r requirements.txt`
3. Run: `streamlit run app.py`

---
*Developed by Akshaya*