# Retrieval-Augmented Generation (RAG) with FAISS and Sentence Transformers

## **Overview**
This project implements a **Retrieval-Augmented Generation (RAG) system** for **semantic search** in medical textbooks. Using **FAISS (Facebook AI Similarity Search)** for efficient similarity retrieval and **Sentence Transformers (MiniLM-L6-v2)** for embedding generation, it allows users to **query medical knowledge** and retrieve the most relevant text snippets.

The system takes raw text from **MIMIC Medical Textbooks**, preprocesses it, converts it into embeddings, and enables **fast similarity-based document retrieval**.

---

## **Dataset Information**
This project processes **MIMIC Medical Textbooks**, which contain structured knowledge related to healthcare topics such as:
- Diseases & Symptoms
- Treatments & Medications
- Clinical Guidelines
- Pathophysiology

**Dataset Details:**
- The dataset consists of **text files (`.txt`)**.
- It is automatically **downloaded from a Dropbox link**.
- Extracted text is **cleaned, chunked, and transformed into embeddings** for efficient retrieval.

---

## **Project Workflow**
1. **Download & Extract Dataset** – Retrieves medical textbook data and stores it in a local directory.
2. **Preprocess Text Data** – Cleans, tokenizes, and chunks text into smaller segments.
3. **Generate Embeddings** – Uses **MiniLM-L6-v2** to convert text into vector embeddings.
4. **Build FAISS Index** – Stores embeddings for fast similarity search.
5. **Query the Search System** – Uses FAISS to find the most relevant text chunks for a given query.

---
