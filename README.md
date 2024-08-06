
# SQLSpeak

SQLSpeak is a sophisticated system designed to convert human language queries into SQL statements, enabling users to retrieve data from a database effortlessly. This project leverages advanced natural language processing and machine learning techniques to bridge the gap between human language and structured database queries.

## Features

- **Natural Language Understanding:** Converts user input in plain English to precise SQL queries.

- **Efficient Data Retrieval:** Executes the generated SQL queries on the database to fetch the required data.

- **Semantic Similarity:** Uses semantic similarity for better understanding and interpretation of user queries.

- **Embeddings and Vector Stores:** Utilizes advanced embeddings and vector stores for accurate and efficient query processing.

## Tech Stack

**Language Model:**

- **Google Palm:** Handles natural language processing and     understanding.
**Database Utility:**

- **SQLDatabase (LangChain):** Facilitates interaction with the SQL database.
**Chain for SQL Queries:**

- **SQLDatabaseChain (LangChain):** Manages the conversion process from natural language to SQL queries.

**Example Selector:**

**SemanticSimilarityExampleSelector (LangChain):** Enhances query understanding by selecting relevant examples based on semantic similarity.

**Embeddings:**

**HuggingFaceEmbeddings:** Provides high-quality embeddings for natural language understanding.

**Vector Store:**

**Chroma:** Stores and retrieves vector representations of text for efficient query processing.

**Prompt Templates:**

- **FewShotPromptTemplate (LangChain):** Utilized for few-shot learning in prompt engineering.
- **PromptTemplate (LangChain):** Custom templates for prompt creation.

**Custom Prompts:**

- **PROMPT_SUFFIX:** Tailored suffix for prompts.
- **_mysql_prompt:** Specific prompt designed for MySQL database interactions.
## How It Works ##

**User Input:** The user inputs a query in natural language.

**Processing:** The input is processed using Google Palm to understand the intent and context.

**Query Conversion:** The processed input is converted into a SQL query using SQLDatabaseChain and other LangChain components.

**Data Retrieval:** The generated SQL query is executed against the database using SQLDatabase, and the results are fetched.

**Response:** The retrieved data is presented to the user in a readable format.
