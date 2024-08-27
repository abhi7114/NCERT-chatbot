# NCERT-chatbot

This project creates a chatbot capable of answering questions based on the NCERT textbooks. It leverages natural language processing techniques to provide informative and relevant responses.

## Key Features:

- **Text Extraction** : Extracts text from NCERT textbooks in PDF format.
- **Sentence Chunking** : Divides extracted text into manageable sentence chunks.
- **Semantic Embedding** : Embeds sentence chunks using the SentenceTransformer model to capture their meaning.
- **Vector Database** : Stores sentence embeddings in a ChromaDB vector database for efficient retrieval.
- **LLM Integration** : Connects to a large language model (LLM) like Gemini to generate responses.
- **Streamlit UI** : Provides a user-friendly interface for interacting with the chatbot.
  
## Workflow:

- Data Ingestion: Loads NCERT textbooks as PDFs.
- Text Extraction: Extracts text from the PDFs.
- Sentence Chunking: Divides text into sentences.
- Embedding: Converts sentences into numerical embeddings using the SentenceTransformer model.
- Vector Database: Stores embeddings in ChromaDB for efficient search.
- User Query: When a user asks a question through the Streamlit interface, the question is embedded using the same SentenceTransformer model.
- Semantic Search: Searches the vector database for the most similar sentence chunks based on the embedded question.
- LLM Response: Provides the top 3 similar sentence chunks as context to the LLM, which generates a response.
- UI Display: Displays the LLM's response in the Streamlit interface.

  
## Technologies Used:

- Python
- TensorFlow (for SentenceTransformer)
- ChromaDB
- Gemini LLM
- Streamlit

## Potential Improvements:

- Contextual Understanding: Enhance the chatbot's ability to understand context and provide more relevant responses.
- Fine-tuning: Fine-tune the LLM on the NCERT dataset to improve its performance on specific topics.
- Evaluation: Develop metrics to evaluate the chatbot's accuracy and effectiveness in answering questions.

This project demonstrates the application of natural language processing and machine learning for creating intelligent chatbots that can provide information from educational resources.
