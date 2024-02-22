# FinanceIQ

Follow these steps to install and run the FinanceIQ project:
1. Clone the repository to your local machine using the following command:
   ```bash
   git clone https://github.com/manan3101/FinanceIQ.git
2. Install necessary dependencies using pip:
   ```bash
   pip install -r requirements.txt
3. Set up your OpenAI API and Modify the .env file to include your API key:
   ```bash
   OPENAI_API_KEY="enter your key"
4. Run the project using Streamlit:
   ```bash
   streamlit run main.py
   ```


Project Workflow
This project operates in two main phases:

Phase 1: Creating Knowledge Base
Data Extraction from URL:

User provides a URL.
The project utilizes UnstructuredURLLoader() to load and extract data from the provided URL article.
The loaded data is then prepared for further processing.
Text Chunking:

The loaded data is split into manageable chunks using split_documents().
This step breaks down the text into smaller sections, facilitating efficient processing.
Embedding Generation:

Embeddings are created for all the text chunks using OpenAIEmbeddings().
Embeddings capture the semantic representations of the text, enabling meaningful analysis.
Vector Database Creation:

A vector database is constructed using FAISS.
This database indexes the embeddings of the text chunks, allowing for fast and effective retrieval of relevant information.






