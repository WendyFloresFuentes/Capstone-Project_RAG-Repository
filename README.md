# 📚 Research Q&A Assistant  
### Retrieval-Augmented Generation (RAG) with Explainable AI (SHAP & LIME)

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Streamlit](https://img.shields.io/badge/Framework-Streamlit-red)
![LangChain](https://img.shields.io/badge/LLM-LangChain-green)
![OpenAI](https://img.shields.io/badge/Model-OpenAI-black)
![ChromaDB](https://img.shields.io/badge/VectorDB-ChromaDB-purple)
![Explainable AI](https://img.shields.io/badge/XAI-SHAP%20%7C%20LIME-orange)

---Overview
The Research Q&A Assistant is an AI-powered interactive web-based academic assistant that allows users to upload research papers (PDFs) and ask domain-specific questions.
The system uses:
	•	Retrieval-Augmented Generation (RAG) for context-aware answering
	•	Large Language Models (LLMs) via OpenAI
	•	Vector embeddings and ChromaDB for semantic search
	•	Explainable AI (XAI) techniques using SHAP and LIME
This capstone project demonstrates how Retrieval-Augmented Generation (RAG) improves answer reliability while maintaining interpretability through Explainable AI techniques.
 
 Problem Statement
Researchers face several challenges such as:
	•	Time-consuming manual search through PDFs
	•	Lack of semantic understanding with keyword-based search
	•	Limited transparency in AI-generated answers
	•	Hallucination of LLMs without grounding
 
Proposed Solution
A RAG-based Research Assistant that:
	1	Extracts text from uploaded research papers
	2	Converts text into semantic embeddings
	3	Stores embeddings in a vector database
	4	Retrieves relevant content using similarity search
	5	Generates context-grounded answers using an LLM
	6	Provides explanation using SHAP & LIME
 
System Architecture
User Uploads PDF
        ↓
Text Extraction (PyPDF / PyPDF2)
        ↓
Chunking (LangChain Text Splitter)
        ↓
Embeddings (Sentence Transformers)
        ↓
Vector Storage (ChromaDB)
        ↓
Similarity Retrieval
        ↓
OpenAI LLM (Answer Generation)
        ↓
SHAP & LIME Explanation
 
Project Structure
Research-QA-Assistant
ProjectApp_RAG.py
ProjectApp_RAG-SHAP-LIME.py
requirements.txt
README.md
 
ProjectApp_RAG.py: Core RAG-based research assistant.
ProjectApp_RAG-SHAP-LIME.py: Extended version with Explainable AI integration.
 
Technical Stack
 
Component
Technology
Frontend
Streamlit
LLM
OpenAI GPT models
Framework
LangChain
Embeddings
Sentence Transformers
Vector DB
ChromaDB
Explainability
SHAP & LIME
Data Handling
Pandas
Visualization
Plotly
 
Installation
1️ Clone the Repository
git clone https://github.com/your-username/Research-QA-Assistant.git
cd Research-QA-Assistant
2️ Create Virtual Environment (Recommended)
python -m venv venv
source venv/bin/activate  # macOS/Linux
3️ Install Dependencies
pip install -r requirements.txt
 
Environment Setup
Set your OpenAI API key:
export OPENAI_API_KEY="your_api_key_here"
 
Running the Application
Run Basic RAG Version
streamlit run ProjectApp_RAG.py
Run RAG + Explainability Version
streamlit run ProjectApp_RAG-SHAP-LIME.py
The app will open at: http://localhost:8501
 
Evaluation Metrics
	•	Answer relevance (qualitative evaluation)
	•	Context retrieval accuracy
	•	Reduction in hallucination
	•	Response coherence
	•	Explainability (SHAP & LIME interpretability)
 
What Worked Well
	•	Strong semantic retrieval performance
	•	Improved reliability using RAG
	•	Interactive Streamlit interface
	•	Enhanced transparency through XAI
 
Challenges & Solutions
 
Challenge
Solution
Large PDF processing
Optimized chunking strategy
Hallucination risk
Retrieval-Augmented Generation
 
Key Learnings
	•	RAG significantly improves LLM reliability
	•	Vector databases are essential for semantic retrieval
	•	Explainability enhances trust in AI systems
	•	System integration is critical for production-ready AI tools
 
Future Improvements
	•	Multi-document comparison
	•	Citation highlighting
	•	Source linking in answers
	•	Fine-tuned domain embeddings
 
Academic Context
This project was developed as a Capstone Project demonstrating:
	•	Generative AI Engineering
	•	Retrieval-Augmented Generation
	•	Explainable AI
	•	Responsible AI system design
 
License
This project is for academic and educational purposes.
