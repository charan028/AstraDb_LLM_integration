# AstraDb_LLM_integration
# AstraDB LangChain Quickstart

This notebook demonstrates how to use **LangChain** with **AstraDB** to build a vector store for storing and querying embeddings. The notebook walks through the process of setting up a vector store, loading a dataset, creating embeddings, and querying them using natural language.

## Overview

This notebook covers:

1. **Environment Setup**:
   - Import required libraries, including `langchain_astradb`, `langchain_core`, and `OpenAIEmbeddings`.
   - Configure your environment with necessary API keys and tokens.

2. **Vector Store Creation**:
   - Initialize an embeddings model using `OpenAIEmbeddings`.
   - Create a vector store in AstraDB using the initialized embeddings model.

3. **Dataset Loading**:
   - Load a small dataset (e.g., philosopher quotes) to test the vector store.
   - Demonstrate how the dataset is structured and preview example entries.

4. **Embedding and Storing Data**:
   - Convert the dataset entries into embeddings.
   - Store the embeddings in the AstraDB vector store.

5. **Querying the Vector Store**:
   - Input natural language queries to search the vector store.
   - Retrieve and display relevant results based on the embeddings.

6. **LangChain Integration**:
   - Set up a basic LangChain pipeline to process user queries.
   - Demonstrate the pipeline with example queries and responses.

7. **Cleanup**:
   - Optionally delete the vector store collection in AstraDB to free resources.

## Prerequisites

To use this notebook, you need:

- Python 3.9 or later.
- AstraDB account and credentials.
- OpenAI API key for generating embeddings.

## Installation

1. export api key in env file:
   ```bash
   export ASTRA_DB_APPLICATION_TOKEN=<your_astra_db_token>
   export ASTRA_DB_API_ENDPOINT=<your_astra_db_endpoint>
   export OPENAI_API_KEY=<your_openai_api_key>

   chain.invoke("How does Russell elaborate on Peirce's idea of the security blanket?")

This README file provides an overview of the notebook, prerequisites, installation steps, and usage instructions. You can customize it further based on your specific needs. &#8203;:contentReference[oaicite:0]{index=0}&#8203;
