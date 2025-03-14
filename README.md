# Text-to-SQL: Natural Language to SQL Conversion with GPT-4o and Fuzzy Matching

Text-to-SQL converts natural language queries into SQL using GPT-4o and advanced fuzzy matching (Jaro-Winkler). It intelligently corrects misspellings, generates accurate SQL queries, ensures secure multi-tenancy, and integrates custom databases like ClickHouse via LangChain.

This repository demonstrates a powerful application that translates natural language queries into accurate and executable SQL statements. Leveraging advanced NLP techniques, fuzzy matching algorithms, and OpenAI’s GPT-4o model, this project simplifies database interactions, making them accessible to non-technical users and business analysts alike.

## **Key Features**

1) Natural Language Processing (NLP): Converts plain English queries to structured database queries.

2) Advanced Spell Correction: Uses GPT-4o and Jaro-Winkler similarity for intelligent typo corrections.

3) Dynamic SQL Query Generation: Automatically generates optimized SQL queries.

4) Robust Error Handling: Implements automatic retries and GPT-based query correction.

5) Secure Multi-Tenancy: Enforces application-specific filtering (application_id) for security.

6) Custom Database Integration: Demonstrates integration with ClickHouse and adaptability to other LangChain-supported databases.


## **Technologies Used**

1) LangChain

2) OpenAI GPT-4o 

3) ClickHouse

4) Jellyfish (Jaro-Winkler Fuzzy Matching)

5) Python 3.9+

## **Installation and Setup** 

### 1. Clone the Repository

```bash
git clone https://github.com/SohamSanyal2000/Text-to-SQL.git
cd text-to-sql
```

### 2. Create a Virtual Environment

```bash
python -m venv env
source env/bin/activate   # Linux/MacOS
.\env\Scripts\activate    # Windows
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Set Up Environment Variables

Create a `.env` file in the root of the project and add your OpenAI API key:

```
OPEN_AI_API_KEY=your_openai_api_key
host=clickhouse_host
port=clickhouse_port
user=clickhouse_user
password=clickhouse_password
database=clickhouse_database
application_id=your_application_id
```
### 5. Example natural-language query:
```
List customers who bought shoes from Adidas and shirts from Nike.
```
