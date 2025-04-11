HEAD
# CSV-to-SQLite-Application-with-AI
This tool converts CSV files into SQLite databases, automatically generating schemas and allowing SQL queries. It also integrates AI to generate SQL queries from natural language, simplifying data analysis. Built with Python, Pandas, SQLite, and OpenAI for AI-assisted querying.

# 🧾 AI Bookeeper

AI Bookeeper is an AI-powered web app that helps you analyze CSV data with natural language. Upload your spreadsheet, ask a question in plain English, and get SQL-powered answers using OpenAI.

---

## ✨ Features

- 📂 Upload any CSV to automatically create a SQLite table
- 🔍 Run SQL queries manually or with AI assistance
- 🧠 Use natural language (e.g. *"What was the total revenue per day?"*)
- ⚡ Instantly see query results in a clean table
- 🔒 AI responses are restricted to safe `SELECT` statements

---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone git@github.com:trevorpoppe/CSV-to-SQLite-Application-with-AI.git
cd CSV-to-SQLite-Application-with-AI/AI-Bookeeper
```

### 2. Set up the environment

```bash
pip install flask openai pandas python-dotenv
```

> Optionally create a `.env` file to hold your OpenAI API key:

```env
OPENAI_API_KEY=sk-...
```

Or export it directly:

```bash
export OPENAI_API_KEY=sk-...
```

### 3. Run the app

```bash
python app.py
```

Then open your browser to http://127.0.0.1:5000

---

## 💡 Example Prompts

Try asking questions like:

- *"What is the total revenue per day?"*
- *"List the number of sales per product_id"*
- *"Show me the average revenue for each product"*

The AI will convert these into SQL and return results instantly.

---

## 🛠 Project Structure

```
AI-Bookeeper/
├── app.py               # Flask app
├── templates/
│   └── index.html       # Web UI
├── uploads/             # Uploaded CSVs
├── bookkeeper.db        # SQLite database
├── sample_data.csv      # Example CSV file
└── README.md
```

---

## 🧹 TODO / Improvements

- [ ] Add support for multi-table joins
- [ ] Enhance AI prompt context with table schema
- [ ] Add CSV column data type preview
- [ ] Pagination for long result sets

---

## 📄 License

MIT License — use it, fork it, make it better.

---

## 🙌 Credits

Built by [Trevor Poppe](https://github.com/trevorpoppe)  
Powered by Flask, SQLite, Pandas, and OpenAI.
>>>>>>> 07a4df1 (Initial commit)
