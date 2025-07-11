# 🧠 Multi-Agent System with LangGraph (LLM-Orchestrated SQL + Python Agents)
This project demonstrates a tool-augmented multi-agent system using LangGraph to coordinate large language model agents across reasoning tasks. It showcases how to construct a modular, LLM-powered workflow for structured data analysis, using a Supervisor Agent to manage interactions between:

- **SQL Agent** – retrieves relevant data from a SQLite database (Chinook) using natural language queries

- **Python Agent** – performs analytical computations (e.g., aggregations, growth rates) on the SQL output

- **Supervisor Agent** – governs the control flow and routes tasks between agents using LangGraph's execution engine

# 🔧 Built With
- LangGraph Supervisor

- LangChain Agents + Toolkits

- Google GenAI (Gemini 2.0 Flash Lite) as the LLM backend

- SQLite (Chinook sample database)

- Python toolchain (PythonREPLTool for in-memory computation)

# 📌 Features
- Graph-based multi-agent orchestration using LangGraph

- Natural-language-to-SQL generation with LLM

- Agent handoff logic (SQL → Python) based on result requirements

- Visual execution graph rendering

- End-to-end traceability of SQL queries and Python reasoning steps

# ✅ Example Use Case
> “Calculate the revenue growth rate for Rock genre between 2009 and 2010.”

The SQL agent queries the database; if a follow-up calculation is needed, the Python agent is automatically triggered. The system returns the final answer along with code used for transparency.
