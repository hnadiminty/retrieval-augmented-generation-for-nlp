
<p align="center">
 # 🔍 Retrieval-Augmented Generation for NLP Research Papers

</p>

![Python](https://img.shields.io/badge/Python-3.10-blue) ![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red) ![Transformers](https://img.shields.io/badge/HuggingFace-Transformers-yellow) ![FAISS](https://img.shields.io/badge/FAISS-Vector%20Search-green) ![License](https://img.shields.io/badge/License-Academic-lightgrey)

A comprehensive **Retrieval-Augmented Generation (RAG)** pipeline for semantic search and citation-backed question answering over NLP research papers.

> This project was completed collaboratively as part of a five-member team, for the course:  CSE 575 – Statistical Machine Learning at Arizona State University

---

## 📖 Overview

This project implements an end-to-end Retrieval-Augmented Generation system that enables users to query Natural Language Processing research papers using natural language.

The pipeline combines **semantic retrieval**, **keyword-based retrieval**, and **large language models** to generate context-aware responses grounded in academic literature.

---

## ✨ Features

* 📄 Download and process NLP papers from arXiv
* 🧩 PDF text extraction and document chunking
* 🔍 Dense Retrieval using **FAISS**
* 📚 Sparse Retrieval using **BM25**
* ⚡ Hybrid Retrieval
* 🤖 Multiple embedding models

  * SciBERT
  * MiniLM
  * MPNet
  * Instructor
* 💬 Answer generation using

  * Flan-T5
  * TinyLlama
* 📖 Citation-aware responses
* 📊 ROUGE & BLEU evaluation
* 📈 Retrieval and scalability analysis

---

## 🏗️ System Architecture

```
                 User Query
                     │
                     ▼
            Query Embedding
                     │
                     ▼
        Hybrid Retrieval Engine
          (FAISS + BM25)
                     │
                     ▼
       Relevant Document Chunks
                     │
                     ▼
        Flan-T5 / TinyLlama
                     │
                     ▼
      Citation-Backed Response
```

---

## 🛠️ Tech Stack

| Category        | Technologies                       |
| --------------- | ---------------------------------- |
| Language        | Python                             |
| Frameworks      | PyTorch, Transformers              |
| Embeddings      | SciBERT, MiniLM, MPNet, Instructor |
| Retrieval       | FAISS, BM25                        |
| Data Processing | NumPy, Pandas                      |
| Visualization   | Matplotlib                         |
| Development     | Google Colab                       |

---

# ⚙️ Installation

## Clone the repository

```bash
git clone https://github.com/hnadiminty/retrieval-augmented-generation-for-nlp.git

cd retrieval-augmented-generation-for-nlp
```

## Create a virtual environment (recommended)

```bash
python -m venv venv
```

Windows

```bash
venv\Scripts\activate
```

macOS / Linux

```bash
source venv/bin/activate
```

## Install dependencies

```bash
pip install -r requirements.txt
```

---

# 🚀 Running the Project

Open the notebook:

```
Retrieval_Augmented_Generation_for_NLP_Research_Papers.ipynb
```

Run the notebook sequentially.

The notebook performs:

* Data preprocessing
* Embedding generation
* FAISS index creation
* BM25 indexing
* Hybrid retrieval
* Response generation
* Evaluation
* Visualization generation

---

## 📂 Repository Structure

```
retrieval-augmented-generation-for-nlp/
│
├── Retrieval_Augmented_Generation_for_NLP_Research_Papers.ipynb
├── Team-1-CSE575.pdf
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 📊 Evaluation

The project evaluates the RAG pipeline using:

* Embedding model comparison
* Hybrid retrieval optimization
* ROUGE
* BLEU
* Retrieval quality
* Query latency
* FAISS scalability

---

## 📄 Report

The complete project report is included in this repository for reference.

---

## 🙏 Acknowledgements

This project was developed for **CSE 575 – Statistical Machine Learning** at **Arizona State University** as a collaborative academic project.
