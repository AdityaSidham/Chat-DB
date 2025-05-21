ChatDB – Natural Language Interface for MySQL and MongoDB

ChatDB is a Streamlit-based application that allows users to query both **relational (MySQL)** and **NoSQL (MongoDB)** databases using **natural language**. It leverages **Google Gemini Pro** (Generative AI) to convert human language into executable database queries.

---

## Features

-  Ask questions in natural language (e.g., “Show all customers from New York”)
-  Gemini converts input into SQL or MongoDB queries
-  Automatic detection of database type
-  Execute queries and view results as tables
-  Supports:
  - MySQL: SELECT, JOIN, INSERT, UPDATE, DELETE, etc.
  - MongoDB: `find`, `$aggregate`, `$lookup`, `insertOne`, `updateOne`, etc.

---

## Prerequisites

##  Setting Up

### Step 1: Clone or Download
```bash
git clone https://github.com/yourusername/ChatDB.git
cd ChatDB
```

### 1. Software Requirements
- [Python 3.8+](https://www.python.org/downloads/)
- [MySQL Server](https://dev.mysql.com/downloads/mysql/)
- [MongoDB Community Edition](https://www.mongodb.com/try/download/community)
- [Google Account for Gemini API](https://ai.google.dev/)

### 2. Python Libraries
Install all dependencies using:

```bash
pip install -r requirements.txt
```

### 3. Google Gemini API Key
- Sign up at: [Google AI Studio](https://makersuite.google.com/app)
- Go to **API Keys**
- Copy your key and **replace it in `chatDB_pt1.py`:** where genai.configure(api_key="your_API_key")  


---


### Step 2: Setup MySQL & MongoDB

-  Create sample databases like:
  - `chatdb`, `educationdb`, `clinicdb` or any in MySQL
  - `ecommerce_mongo`, `university_mongo`, `clinic_mongo` or any in MongoDB 
-  Import your sample `.csv` or `.json` data in the ChatDB application 

### Step 3: Run the App

```bash
streamlit run chatDB_pt1.py
```

---

##  Project Structure

```
chatDB/
│
├── chatDB_pt1.py          # Main Streamlit app
├── requirements.txt       # Required Python packages
├── README.md              # You’re reading this
└── data/                  # CSV and JSON files for demo
```

---

Thank You!!



