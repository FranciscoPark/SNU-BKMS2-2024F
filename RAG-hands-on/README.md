# BKMS2 Hands-on #4: Developing a Q&A chatbot based on RAG
- **Date**: 2024.10.15.
- **Instructor**: Prof. Sang-Won Lee
- **TA**:         Kun-Woo Shin (kunwooshin@snu.ac.kr)

## Overview
In this hands-on session, we will implement the fundamental components of the Retrieval-Augmented Generation (RAG) process, as discussed in previous lessons. Afterward, we will replicate the same process using LangChain to understand how it simplifies the creation of RAG-based chatbot applications.

The data for this session is collected from the Graduate School of Data Science (GSDS) website and file shared on the Slack channel. Using this data, we will build a simple RAG-based Q&A chatbot of GSDS.


<p align="center">
  <img width="70%" src="https://github.com/user-attachments/assets/a590a8c9-9a95-4bc2-89e4-26c049028e75">
</p>

To ensure consistency in the Python module dependencies for this hands-on exercise, we will be using **Google Colab**.

1. **Download the notebook**: Download the `BKMS2_hands_on_4.ipynb` file from this repository.
2. **Open in Colab**: Upload and open the notebook in Google Colab.

## Requirements
Before the class, follow the setup instructions below in your Google Colab environment and test whether everything works correctly. If it doesn’t work properly, contact the TA for assistance.​

An API key for OpenAI models is not required, as you will be provided with a key during the session.​
The key is only available during the session and will expire once the session ends. _**Please do not use it for any job other than calling the models specified in the given code.**_

## Setup

1. **Load `data.zip`**: Download `data.zip` from this directory and upload it in your Colab notebook

3. **Unzip the file**: Unzip the data by running the following command in Colab:

    ```bash
    !unzip /content/data.zip -d /content
    ```

4. **Install dependencies**: Install the required Python packages listed in the `requirements.txt` file:

    ```bash
    !pip install -r /content/data/requirements.txt
    ```
5. **Download `punkt` module**: Run the following command to download necessary NLTK module:
   ```bash
   import nltk
   nltk.download('punkt')

## References
#### Chroma DB
Guides for ChromaDB: https://docs.trychroma.com/guides

#### LangChain
Guides for LangChain: https://python.langchain.com/docs/how_to/

- **Vector Stores**: https://python.langchain.com/docs/integrations/vectorstores/
- **Retrievers**: https://python.langchain.com/docs/integrations/retrievers/
  
Another tutorial on RAG using LangChain: https://python.langchain.com/docs/tutorials/rag/

