# Deep Learning in Legal System: Opportunities and Challenges

> My bachelor thesis on applying AI, deep learning, and information retrieval to Vietnamese legal documents.  
> Final thesis score: **9.7/10**.

This repository contains the source code, thesis document, and presentation for my bachelor thesis:

**Deep Learning in Legal System: Opportunities and Challenges**  
**Author:** Ngô Phú Thịnh  
**Major:** Data Science  
**University:** University of Science, Vietnam National University Ho Chi Minh City  
**Supervisor:** Assoc. Prof. Dr. Nguyễn Thanh Bình  
**Year:** 2023

## About This Thesis

This was my bachelor thesis in Data Science. I researched how modern AI systems, especially large language models and retrieval-based methods, can be applied to the legal domain.

The main idea behind this project was simple: **law should be easier to access and understand**.

In Vietnam, legal documents can be difficult for ordinary users to search, read, and understand. I wanted to explore how AI could support citizens, law students, legal researchers, and lawyers by making legal information retrieval more efficient.

The thesis has two main parts:

1. A research discussion about the opportunities and challenges of deep learning in legal systems.
2. Practical experiments on Vietnamese legal document retrieval.

## Thesis Score

I received **9.7/10** for this thesis.

## Main Topics

- Legal AI
- Large Language Models
- GPT and ChatGPT
- Embeddings
- TF-IDF
- BM25
- Sentence Transformers
- ChromaDB
- LangChain
- Open-Domain Question Answering
- Multimodal AI
- Vietnamese legal document retrieval
- AI challenges in law: privacy, cost, hallucination, ethics, and reliability

## What I Built

The practical part of the thesis focused on building and testing a retrieval system for Vietnamese legal documents.

Main components:

### 1. Vietnamese Legal Document Dataset

I collected and processed Vietnamese legal normative documents, mainly related to social insurance.

### 2. Legal Document Database

I designed a database structure to store:

- Legal documents
- Document metadata
- Table of contents
- Relationships between legal documents
- Processed legal text

### 3. Vietnamese Legal Question-Answering Dataset

I prepared legal Q&A data for retrieval experiments and fine-tuning.

### 4. Information Retrieval Experiments

I tested several retrieval methods:

- TF-IDF
- BM25
- Dense embedding retrieval
- Instructor Embedding models
- Fine-tuned Instructor Embedding model
- ChromaDB vector search

## Key Result

One important result was that fine-tuning significantly improved retrieval performance.

In the second retrieval approach, the original Instructor models performed poorly on the Vietnamese legal dataset. After fine-tuning, the Instructor Base model achieved much better results.

| Model | Top 5 Accuracy | Top 10 Accuracy | Top 20 Accuracy | Top 50 Accuracy |
|---|---:|---:|---:|---:|
| INSTRUCTOR-BASE | 0.0119 | 0.0221 | 0.0416 | 0.0944 |
| INSTRUCTOR-LARGE | 0.0138 | 0.0247 | 0.0421 | 0.1023 |
| INSTRUCTOR-XL | 0.0188 | 0.0312 | 0.0537 | 0.1427 |
| INSTRUCTOR-BASE FTS1 | 0.4832 | 0.5741 | 0.6621 | 0.7765 |
| INSTRUCTOR-BASE FTS2 | 0.6431 | 0.7432 | 0.8123 | 0.8912 |

This showed that domain-specific fine-tuning can greatly improve retrieval quality, even with limited hardware and a smaller model.

## Repository Structure

```txt
.
├── code/              # Source code and experiments
├── document/          # Thesis document and related files
├── LuanVan.pptx       # Thesis presentation
└── readme.md          # Repository overview
```

## Technologies Used

- Python
- Jupyter Notebook
- TF-IDF
- BM25
- Sentence Transformers
- Instructor Embedding
- ChromaDB
- LangChain
- Pandas
- NumPy
- Streamlit
- Typst

## Thesis Document

Thesis PDF:

```txt
document/thesis.pdf
```

Presentation:

```txt
LuanVan.pptx
```

## Keywords

Vietnamese legal AI, Vietnamese legal question answering, Vietnamese law retrieval, legal information retrieval, Vietnamese NLP, AI for law, legal document search, BM25, TF-IDF, ChromaDB, Instructor Embedding, Sentence Transformers, legal RAG, deep learning legal system, AI in legal system.

## Citation

```bibtex
@thesis{ngo2023legalai,
  title  = {Deep Learning in Legal System: Opportunities and Challenges},
  author = {Ngo Phu Thinh},
  year   = {2023},
  school = {University of Science, Vietnam National University Ho Chi Minh City},
  type   = {Bachelor Thesis},
  url    = {https://github.com/Th1nhNg0/luanvantotnghiep}
}
```

## Author

**Ngô Phú Thịnh**

- GitHub: [Th1nhNg0](https://github.com/Th1nhNg0)
- Website: [thinhcorner.com](https://thinhcorner.com)

## Notes

This was an academic thesis project built with limited time, hardware, and data. The project can be improved further with larger datasets, stronger embedding models, better Vietnamese legal corpora, and more advanced retrieval methods such as Dense Passage Retrieval or modern RAG pipelines.
