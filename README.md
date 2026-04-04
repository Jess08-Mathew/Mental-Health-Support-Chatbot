
---

# 🧠 Mental Health Chatbot (RAG-Based Conversational AI)

## 🚀 Overview
Built an end-to-end **Retrieval-Augmented Generation (RAG)** system to improve response quality in mental health conversations. The chatbot retrieves relevant context from a knowledge base and uses it to generate grounded, consistent, and empathetic responses.

## 🧠 Problem
Standard LLM-based chatbots:
- Produce generic responses  
- Lack contextual grounding  
- Do not leverage external knowledge  

This project addresses these gaps using a **retrieval + generation pipeline**.

## 🏗️ Architecture
- **Retriever** → Fetches relevant context from vector database  
- **LLM** → Generates responses using retrieved context  
- **Pipeline** → Ensures grounded and context-aware outputs  

## ⚙️ Core Components

**LLM Layer**
- Groq (LLaMA 3) via `langchain_groq`  
- Deterministic configuration (low temperature)

**Retrieval System**
- LangChain `RetrievalQA`  
- Context injection into prompts  

**Embeddings**
- HuggingFace `all-MiniLM-L6-v2`  
- Semantic similarity search  

**Vector Database**
- ChromaDB with persistent storage  

**Data Pipeline**
- PDF ingestion (`PyPDFLoader`)  
- Text chunking (`RecursiveCharacterTextSplitter`)  

**Interface**
- Gradio ChatInterface for real-time interaction  

## 🔄 Workflow

User Query → Semantic Retrieval → Context Injection → LLM → Response


## 🔑 Features
- Context-aware response generation  
- Retrieval-augmented architecture  
- Semantic search over documents  
- Modular and scalable pipeline  
- Interactive chatbot interface



## 🏗️ Tech Stack
- **LLM:** Groq (LLaMA 3)  
- **Framework:** LangChain  
- **Embeddings:** HuggingFace  
- **Vector DB:** ChromaDB  
- **UI:** Gradio  
- **Language:** Python  

## 📌 Key Takeaways
- Designed and implemented a production-style **RAG pipeline**  
- Improved response grounding using retrieval mechanisms  
- Built a modular system combining LLMs and vector search  
- Developed an end-to-end AI application

## Code 
👉 *https://colab.research.google.com/drive/1hcbNd04F3yWgCWcTQTgEw_Eo5Ad9-A0n#scrollTo=HxQR6_wVcjS9*

## ⚠️ Disclaimer
This project is a technical prototype and not a substitute for professional mental health support.
