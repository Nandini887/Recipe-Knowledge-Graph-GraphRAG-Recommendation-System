# Recipe-Knowledge-Graph-GraphRAG-Recommendation-System
Built an end-to-end GraphRAG pipeline that transforms recipe data into a knowledge graph using LLM-based extraction, enabling semantic search and natural language Q&amp;A through Neo4j and Streamlit.

---

## Overview
This project develops an end-to-end GraphRAG system for intelligent recipe discovery and question answering. The system converts structured and unstructured recipe data into a knowledge graph, enabling semantic search, relationship exploration, and natural language querying. It integrates large language models, Neo4j, and Streamlit to create a scalable and interactive data application.

---

## Key Features
- Knowledge graph with multiple node types and relationship types representing recipes, ingredients, users, and reviews
- LLM-based triple extraction and ingredient substitution generation
- Graph-based semantic retrieval using Neo4j
- Natural language question answering using a GraphRAG pipeline
- Interactive dashboard for dataset analytics
- Streamlit application for real-time recipe discovery

---

## System Architecture

### Data Preprocessing
- Load and clean recipe and interaction datasets
- Normalize ingredients and extract cuisine and dietary information
- Merge datasets to create a unified dataset

### Knowledge Graph Construction
- Design schema for recipes, ingredients, users, and relationships
- Use LLMs to extract triples and generate additional knowledge
- Create structured graph data

### Neo4j Graph Database
- Store nodes and relationships in Neo4j
- Apply constraints and indexes
- Use Cypher queries for validation and exploration

### GraphRAG Question Answering
- Extract entities from user queries
- Generate Cypher queries
- Retrieve results from Neo4j
- Generate natural language responses using LLM

### Application Layer
- Streamlit-based interface
- Allows users to input queries and filter results
- Displays recommended recipes with explanations

---

## Knowledge Graph Schema
- Node types include Recipe, Ingredient, Cuisine, DietaryRestriction, Tag, NutritionProfile, User, and Review
- Relationships capture interactions such as ingredient usage, cuisine classification, dietary fit, reviews, and substitutions

---

## Example Query

Input:
Vegetarian Italian dishes under 30 minutes

Process:
- Extract entities such as diet, cuisine, and time
- Generate Cypher query
- Retrieve matching recipes from Neo4j
- Generate response using LLM

Output:
List of relevant recipes with details

---

## Data Details
- 231K recipes
- 1.1M+ user reviews
- 35+ cuisines
- 21 dietary flags

Includes:
- Recipe metadata
- Ingredients
- Cooking steps
- Ratings and reviews

---

## Tech Stack
- Python
- Pandas
- Neo4j
- Cypher
- Large Language Models
- Streamlit

---

## Key Contributions
- Designed and implemented a scalable knowledge graph schema
- Developed LLM-based extraction pipeline
- Built GraphRAG system for semantic search and question answering
- Enabled graph-based recommendations and filtering
- Developed an end-to-end interactive application

---

## Future Improvements
- Add personalization using user behavior
- Enable real-time data ingestion
- Optimize graph query performance
- Extend support for image-based inputs
