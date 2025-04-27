# Neo4j Query Bot with OpenAI API

## Overview
This project is a Neo4j Query Bot that leverages the OpenAI API to process natural language queries and translate them into Cypher queries for interacting with a Neo4j database. The bot simplifies database interactions by allowing users to query using plain English.

## Features
- Natural language processing using OpenAI API.
- Automatic translation of queries into Cypher.
- Integration with Neo4j for database operations.
- Easy-to-use interface for querying and retrieving data.

## Prerequisites
- Python 3.8 or higher
- Neo4j database (local or remote)
- OpenAI API key

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/your-repo/neo4j-query-bot.git
    cd neo4j-query-bot
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Set up environment variables:
    - `OPENAI_API_KEY`: Your OpenAI API key.
    - `NEO4J_URI`: URI for your Neo4j database.
    - `NEO4J_USER`: Username for Neo4j.
    - `NEO4J_PASSWORD`: Password for Neo4j.

    Example `.env` file:
    ```
    OPENAI_API_KEY=your_openai_api_key
    NEO4J_URI=bolt://localhost:7687
    NEO4J_USER=neo4j
    NEO4J_PASSWORD=your_password
    ```

## Usage
1. Start the bot:
    ```bash
    python main.py
    ```

2. Enter natural language queries, and the bot will return results from the Neo4j database.

## Example Query
- Input: "Find all movies directed by Christopher Nolan."
- Output: A list of movies directed by Christopher Nolan from the Neo4j database.

## Project Structure
```
neo4j-query-bot/
├── main.py          # Entry point for the bot
├── query_processor/ # Handles query translation and execution
├── requirements.txt # Python dependencies
├── README.md        # Project documentation
└── .env             # Environment variables
```

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request.


## Acknowledgments
- [Neo4j](https://neo4j.com/) for the graph database platform.
- [OpenAI](https://openai.com/) for the natural language processing API.
- Inspiration from the developer community.
