# Movie Recommendation System

This project implements a robust movie recommendation system that leverages various machine learning and data science techniques to provide personalized recommendations. It combines a graph database for relationship mapping, vector embeddings for semantic similarity, and reranking for enhanced recommendation accuracy.

## Overview

The system is designed to recommend movies based on multiple components such as movie titles, overviews, genres, casts, and directors. The recommendation process involves several steps:

1. **Mapping Relationships**: Using a graph database (Neo4j) to map the relationships between movies, genres, casts, and directors.
2. **Vectorization of Movie Titles and Overviews**: Utilizing HuggingFace's Word2Vec model to convert movie titles and overviews into vector representations.
3. **Semantic Search**: Storing the vectors in a Weaviate vector database to perform semantic searches based on user queries.
4. **Reranking with Cohere**: Applying Cohere's rerank API to rerank the initial search results and improve the quality of recommendations.

## Features

- **Graph Database for Relationship Mapping**: Neo4j is used to store and query relationships between movies, genres, casts, and directors.
- **Semantic Vector Search**: HuggingFace’s Word2Vec model generates vectors for movie titles and overviews, stored in Weaviate for efficient semantic search.
- **Enhanced Recommendations**: Cohere's rerank API refines search results to enhance recommendation accuracy.

## Technology Stack

- **Django**: Web framework used to build the application.
- **Neo4j**: Graph database for storing and querying relationships.
- **Weaviate**: Vector database for storing movie vectors and performing semantic searches.
- **HuggingFace Transformers**: Library for generating word embeddings using Word2Vec.
- **Cohere API**: API used for reranking search results to improve recommendation quality.
- **Python**: Programming language used for development.
- **HTML/CSS**: Frontend technologies used to display the recommendations.

## Installation

To get started with the project, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/your_username/movie-recommendation-system.git
   cd movie-recommendation-system
