# Mental-Health-Support-Chatbot
A RAG-based conversational AI system designed to provide context-aware and empathetic mental health responses using external knowledge sources.

🧠 Problem

Traditional chatbots:

Lack context awareness
Generate generic responses
Cannot use external knowledge

This system addresses these limitations using retrieval-augmented generation (RAG).

🏗 Architecture
LLM Layer → Generates responses
Retriever → Fetches relevant context
Vector Store → Stores embeddings
Pipeline → Combines retrieval + generation

⚙️ System Components
🤖 LLM Layer
Groq (LLaMA 3) via langchain_groq
Low temperature for consistent outputs

📄 Document Ingestion
PDF-based knowledge loading (PyPDFLoader)
Scalable document input

✂️ Text Processing
RecursiveCharacterTextSplitter
Chunking for better retrieval

🔍 Embeddings
all-MiniLM-L6-v2 (HuggingFace)
Converts text into vectors

🗄 Vector Database
ChromaDB
Persistent semantic storage

🔗 Retrieval + QA
LangChain RetrievalQA
Context injection into prompts

🧾 Prompt
You are a compassionate mental health chatbot. Respond thoughtfully:

{context}

User: {question}
Chatbot:
🌐 Interface
Gradio ChatInterface
Real-time interaction
🔄 Workflow

User Query → Retrieve Context → Inject into Prompt → LLM → Response

🔑 Features
Context-aware responses
Semantic search
PDF knowledge ingestion
Emotion-focused prompting
Interactive UI

🏗 Tech Stack
LLM: Groq (LLaMA 3)
Framework: LangChain
Embeddings: HuggingFace
Vector DB: ChromaDB
UI: Gradio
Language: Python

📌 Key Learnings
RAG pipeline design
Vector databases & embeddings
Context-aware AI systems
End-to-end application development

⚠️ Note

This project is a technical prototype and not a substitute for professional mental health support.
