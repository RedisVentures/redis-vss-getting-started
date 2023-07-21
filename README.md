# Similarity Search with Redis as a Vector Database

## Overview

The enclosed Jupyter notebook demonstrates how to do semantic searches on unstructured data using vector similarity and Redis. It covers:

- Generating vector embeddings for text data using SentenceTransformers
- Storing JSON documents containing text and vector embeddings in Redis
- Creating a RediSearch index on the JSON data
- Performing semantic searches using vector similarity queries
- Query types demonstrated:
  - KNN similarity search
  - Hybrid search using filters
  - Range queries

The notebook includes code and examples using a synthetic dataset of bicycle descriptions.

## Setup

The notebook requires the following packages:

- **redis (redis-py)**: https://pypi.org/project/redis/
- **sentence_transformers**: https://pypi.org/project/sentence-transformers/
- **pandas**: https://pypi.org/project/pandas/
- **numpy**: https://pypi.org/project/numpy/

You will need access to a running Redis Stack instance. The notebook includes setup code to run Redis Stack in a Colab notebook.

Alternatively, you can run Redis Stack locally using Docker.

## Running the Notebook

To run the notebook end-to-end, simply execute the cells in order.

The key steps are:

1. Load and inspect the sample JSON data
2. Generate vector embeddings for the text descriptions
3. Save the JSON data with embeddings into Redis
4. Create a RediSearch index on the data
5. Execute vector similarity search queries

The notebook includes ample comments explaining each section.

## Key Concepts

The core concepts covered include:

- Using pre-trained NLP models like SentenceTransformers to generate semantic vector representations of text
- Storing and indexing vectors along with structured data in Redis
- Utilizing vector similarity KNN search and other query types in RediSearch
- Ranking and retrieving results by semantic similarity

The techniques presented allow for building powerful semantic search experiences over unstructured data with Redis.