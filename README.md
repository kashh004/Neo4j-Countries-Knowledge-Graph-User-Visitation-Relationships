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

To install the required Python library:

```bash
pip install py2neo
