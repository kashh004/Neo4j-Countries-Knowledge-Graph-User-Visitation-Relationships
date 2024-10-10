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
Project Structure

	•	neo4j_countries_knowledge_graph.ipynb: Jupyter notebook containing the Python code that builds the knowledge graph using Neo4j.
	•	README.md: This file that describes the project.

Data Model

	•	Users: Represent individuals who visit different countries (e.g., Alice, Bob, Carol).
	•	Countries: Represent the countries visited by users (e.g., France, Germany, Japan).
	•	Continents: Represent the continents that countries belong to (e.g., Europe, Asia, South America).
	•	Languages: Represent the official languages spoken in each country (e.g., French, German, Japanese).

Relationships

	•	VISITED: Between User and Country (e.g., Alice -> VISITED -> France).
	•	BELONGS_TO: Between Country and Continent (e.g., France -> BELONGS_TO -> Europe).
	•	SPEAKS: Between Country and Language (e.g., France -> SPEAKS -> French).


To install the required Python library:

```bash
pip install py2neo
