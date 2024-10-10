# Neo4j Countries Knowledge Graph

This project demonstrates how to build a knowledge graph using **Neo4j** to model the relationships between users, countries, continents, and languages. The users are linked to countries they have visited, and the countries are associated with their respective continents and official languages.

## Features

- **Users** visit different **Countries** (represented by a `VISITED` relationship).
- **Countries** belong to specific **Continents** (represented by a `BELONGS_TO` relationship).
- **Countries** have official **Languages** (represented by a `SPEAKS` relationship).
- Simple queries to find countries visited by a user, recommend countries by continent, or by language.

## Requirements

- Python 3.x
- Neo4j Database (with credentials and URL for access)
- `py2neo` Python library

# Knowledge Graph Project

## Project Structure
- **knowledge_graph.py**: Contains the main implementation for creating and managing the knowledge graph using Neo4j.
- **requirements.txt**: Contains the list of required Python packages for the project.
- **README.md**: Instructions for setting up and using the project.

## Prerequisites

### Neo4j
1. Install Neo4j on your local machine. You can download it from the [Neo4j Download Center](https://neo4j.com/download/).
2. Start Neo4j and ensure it's running on `localhost:7687`.
3. Set the default Neo4j username and password (usually `neo4j` and `password`).

### Python
Ensure you have Python 3.x installed on your machine. You can download it from [Python's official website](https://www.python.org/downloads/).

## Usage

### Configure Neo4j Credentials
Open the `knowledge_graph.py` file and modify the following line if your Neo4j server uses different credentials:
```python
kg = KnowledgeGraph(uri="bolt://localhost:7687", user="neo4j", password="your_password")
