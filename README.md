# Financial Research Assistant with Augmented Query Expansion

## Project Description

This project builds a financial research assistant capable of answering complex finance-related questions by extracting insights from financial reports. The system leverages Natural Language Processing (NLP), machine learning models, and a combination of text preprocessing, embeddings, and query expansion to deliver precise and contextually relevant answers to user queries.

The project is designed to handle multiple text files, in this case, 10 news articles, and allows for detailed analysis through:

- Text extraction from PDF reports.
- Splitting long texts into chunks for easier processing.
- Converting text into embeddings (vector representations) using pre-trained models.
- Using ChromaDB to store and query embeddings.
- Generating augmented queries to improve search results and answer relevance.
- Visualizing document embeddings in a lower-dimensional space using UMAP.

## Features

- **Text Extraction & Preprocessing**: Extracts and cleans the text from PDF documents, filters out empty text, and splits large texts into manageable chunks.
  
- **Embedding & Vector Search**: Embeds the text into vector space using Sentence-Transformers, then stores and queries this data using ChromaDB for semantic search.
  
- **Augmented Query Expansion**: Enhances user queries by generating related questions to refine results and improve the search process.
  
- **Visualizing Document Embeddings**: Projects high-dimensional embeddings into a 2D space using UMAP, enabling a clear visualization of document clusters and query relevance.
  
## Requirements

To run the project, you'll need the following dependencies:

- `pypdf` - For extracting text from PDF files
- `chromadb` - For storing and querying document embeddings
- `groq` - To interact with Groq's API for generating augmented queries
- `langchain` - For text splitting and processing
- `matplotlib` - For visualizing the results in 2D space
- `numpy` - For numerical operations
- `umap-learn` - For dimensionality reduction

## Project Output

- **Query Results**: The system will output answers based on the retrieved documents from the ChromaDB query.
- **Augmented Queries**: A list of related questions that are generated to help refine the user's original query.
- **Visualizations**: The script will generate a plot that visualizes the embeddings of the documents, original query, augmented queries, and retrieved answers in a 2D space using UMAP.

## Future Improvements

- Integration of more sophisticated query generation and retrieval mechanisms.
- Deployment of the model as a web app for real-time use.
- Optimizing the embeddings and reducing dimensionality further for better search results.

---
