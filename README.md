# 🔬 Automatic Scientific Researcher (PyTorch-Based)

An **AI-powered scientific discovery platform** that ingests biomedical literature, builds a **citable knowledge graph**, and applies **deep learning models in PyTorch** to generate *novel hypotheses*. Unlike a chatbot, this system combines **transformers (NER + summarization), graph neural networks, and retrieval-based Q&A** into an end-to-end deployable platform.

---

## 🌟 Overview

Modern science produces overwhelming amounts of research. The **Automatic Scientific Researcher** is designed to help:  

- **Extract facts** (genes, diseases, drugs) from thousands of biomedical papers.  
- **Summarize findings** using abstractive models.  
- **Store knowledge in a graph database** with citations to source papers.  
- **Predict novel associations** with Graph Neural Networks (PyTorch Geometric).  
- **Answer complex queries** with Retrieval-Augmented Generation (RAG), always citing original sources.  

---

## 🚀 Key Features

- **📚 Data Ingestion**
  - Fetch and preprocess biomedical abstracts via PubMed API.  

- **📝 Information Extraction (PyTorch)**
  - Fine-tuned BioBERT for Named Entity Recognition (genes, diseases).  
  - Fine-tuned PEGASUS for abstractive summarization.  

- **🧩 Knowledge Graph**
  - Entities and relationships stored in Neo4j.  
  - Every edge is linked back to its PubMed ID.  

- **🔮 Hypothesis Generation (PyTorch Geometric)**
  - GraphSAGE / GAT for link prediction.  
  - Suggests novel gene–disease or drug–disease connections.  

- **💬 Trustworthy Q&A**
  - Dense retrieval using a PyTorch-trained bi-encoder.  
  - RAG pipeline ensures every answer is verifiable with citations.  

- **⚙️ Engineering & Deployment**
  - FastAPI backend serving PyTorch models.  
  - Streamlit frontend with interactive graph queries.  
  - Docker-compose for reproducibility.  

---

## 🧭 Project Roadmap (High-Level)

1. **Data Engineering** → Ingest & clean PubMed abstracts.  
2. **NER Model (PyTorch)** → Fine-tune BioBERT for entity extraction.  
3. **Summarization Model (PyTorch)** → Fine-tune PEGASUS for abstractive summaries.  
4. **Knowledge Graph** → Construct graph in Neo4j with citations.  
5. **Hypothesis Engine (PyTorch Geometric)** → Train GNN for link prediction.  
6. **Dense Retrieval (PyTorch)** → Train SciBERT bi-encoder for semantic search.  
7. **Q&A Interface** → Retrieval + RAG integration.  
8. **Deployment** → FastAPI + Streamlit + Docker.  

---

## 📊 Tech Stack

- **Core ML/DL:** PyTorch, Hugging Face Transformers, PyTorch Geometric  
- **Graph Database:** Neo4j (Cypher queries)  
- **APIs & Serving:** FastAPI  
- **Frontend:** Streamlit  
- **DevOps:** Docker, Git  

---

## 📌 Example Use Cases

- *“Suggest possible drugs for rare diseases based on underexplored literature.”*  
- *“Summarize 500+ papers on a protein family into concise knowledge.”*  
- *“Predict novel gene–disease associations for hypothesis generation.”*  

---

## 📂 Repository Structure


├── data/\
├── notebooks/\
├── src/\
│ ├── ingestion/\
│ ├── nlp/\
│ ├── graphs/\
│ ├── api/\
│ ├── retrieval/\
│ └── ui/\
├── docker/\
└── README.md 
