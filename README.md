🧠 NL2SQL Chatbot using Gemini + PostgreSQL
📌 Overview

This project is an AI-powered application that converts natural language questions into SQL queries, executes them on a PostgreSQL database, and returns both structured results and natural language responses. It leverages Google Gemini via LangChain for SQL generation and explanation, integrated into an interactive Streamlit interface.

🚀 Features
Natural language to SQL conversion (NL2SQL)
Google Gemini LLM integration via LangChain
Automatic PostgreSQL schema extraction
Secure and dynamic SQL execution
Query result visualization using Pandas DataFrames
Natural language explanation of query results
Interactive web UI built with Streamlit
🏗️ System Workflow
User enters a natural language question
Database schema is extracted from PostgreSQL
Gemini generates an SQL query based on schema + question
SQL query is executed on the database
Results are returned as a structured DataFrame
Gemini converts results into a human-readable answer

🧰 Tech Stack
Python
Streamlit
PostgreSQL
SQLAlchemy
LangChain
Google Gemini API
Pandas

📂 Project Structure
nl2sql-chatbot-gemini/
│
├── app.py
├── .env
├── requirements.txt
└── README.md
⚙️ Setup Instructions
1. Clone the repository
git clone https://github.com/your-username/nl2sql-chatbot-gemini.git
cd nl2sql-chatbot-gemini
2. Create virtual environment
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows
3. Install dependencies
pip install -r requirements.txt
4. Configure environment variables

Create a .env file in the root directory:

GOOGLE_API_KEY=your_google_gemini_api_key
DB_URL=postgresql+psycopg2://username:password@host:port/dbname
5. Run the application
streamlit run app.py
💡 Example Queries
Show total sales per month
List top 5 customers by revenue
How many orders were placed in 2024?
Average order value per region
🧠 Technical Highlights
Dynamic schema extraction from PostgreSQL information schema
Prompt engineering for accurate SQL generation
Automatic SQL sanitization for PostgreSQL compatibility
Date/time column handling for analytical queries
LLM-based transformation of SQL results into natural language

📌 Future Improvements
Add SQL validation and safety layer
Support multiple databases (MySQL, SQLite)
Add authentication system
Add query history tracking
Improve few-shot prompting for better SQL accuracy

👩‍💻 Author

Dana Ahmed
Computer Science Graduate
Building AI systems in NLP, Computer Vision, and LLM applications
