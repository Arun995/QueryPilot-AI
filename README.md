# QueryPilot AI — Natural Language SQL Database Assistant

QueryPilot AI is an LLM-powered application that allows users to interact with structured databases using natural-language questions instead of writing SQL queries manually. It uses LangChain's SQL agent toolkit and a Groq-hosted language model to help users retrieve information from SQLite and MySQL databases through a Streamlit interface.

## Features

- **Natural-Language Database Querying:** Ask questions about database contents using everyday language.
- **LLM-Powered SQL Agent:** Uses LangChain's SQL agent toolkit to interpret questions and interact with databases.
- **Multiple Database Support:** Supports SQLite and MySQL through SQLAlchemy.
- **Interactive Web Interface:** Provides a simple conversational interface built with Streamlit.
- **Groq LLM Integration:** Uses a language model hosted by Groq to power query generation and reasoning.

## Tech Stack

- **Language:** Python
- **LLM Integration:** Groq
- **LLM Framework:** LangChain
- **Database Connectivity:** SQLAlchemy
- **Databases:** SQLite, MySQL
- **Frontend:** Streamlit

## How It Works

1. The user provides a database connection and asks a question in natural language.
2. The application connects to the selected database.
3. LangChain's SQL agent toolkit uses the configured language model to interpret the question and interact with the database.
4. The application displays the resulting response through the Streamlit interface.

## Project Structure

```text
QueryPilot-AI/
├── app.py
├── requirements.txt
├── .env.example
└── README.md
```

*Adjust the project structure above to match the actual files in your repository.*

## Getting Started

### Prerequisites

- Python 3.10 or a compatible version supported by your dependencies
- A Groq API key
- Access to a SQLite database or a MySQL database

### 1. Clone the Repository

```bash
git clone <YOUR_REPOSITORY_URL>
cd QueryPilot-AI
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it:

**Windows**
```bash
venv\Scripts\activate
```

**macOS / Linux**
```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Create a `.env` file or use the API-key input provided by the application, depending on how your implementation handles credentials.

Example `.env` configuration, if supported:

```env
GROQ_API_KEY=your_groq_api_key
```

Never commit your real API key to GitHub.

### 5. Run the Application

```bash
streamlit run app.py
```

Open the local URL displayed in the terminal.

## Use Cases

- Exploring database records without manually writing SQL.
- Answering questions about structured business data.
- Demonstrating LLM-powered database interaction.
- Prototyping natural-language interfaces for SQL databases.

## Limitations

- The quality of generated queries and answers depends on the language model, database schema, and available data.
- Database access depends on valid connection details and compatible database configuration.
- Generated SQL and database operations should be reviewed carefully. Use read-only database credentials when possible, particularly when working with important data.

## Future Improvements

- Add SQL query validation and read-only execution safeguards.
- Improve error handling for invalid queries and database connection failures.
- Add schema-aware query examples and query-history support.
- Create automated tests for query generation and database interactions.
- Add evaluation cases to measure answer correctness and reliability.

## Learning Outcomes

This project explores practical LLM application development, natural-language-to-SQL workflows, LangChain SQL agents, database connectivity, and interactive AI application development.

## Author

**Arun Arumugam**

Aspiring AI/ML Engineer | Python | Machine Learning | Generative AI | LLM Applications
