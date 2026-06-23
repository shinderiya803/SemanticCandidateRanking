# SemanticCandidateRanking
AI-powered semantic candidate ranking system using Sentence Transformers and cosine similarity for intelligent talent discovery and job-candidate matching.


## Overview

Recruiters often deal with thousands of resumes for a single job opening. Traditional keyword-based search fails to capture the true meaning of candidate profiles and job descriptions.

This project uses **Sentence Transformers** and **cosine similarity** to understand semantic relationships between candidate profiles and job requirements, enabling more relevant candidate recommendations.

---

## Problem Statement

Given a job description and a large pool of candidate profiles, rank candidates according to their relevance and generate the Top-100 recommendations.

---

## Approach

### 1. Data Preprocessing

* Load candidate dataset.
* Filter candidate profiles.
* Convert structured profile information into textual format.

### 2. Embedding Generation

Generate vector representations using:

* **Sentence Transformers**
* **Model:** `all-MiniLM-L6-v2`

### 3. Similarity Computation

Calculate semantic similarity between:

* Job description embedding
* Candidate profile embeddings

using **Cosine Similarity**.

### 4. Candidate Ranking

Sort candidates according to similarity scores and generate ranked recommendations.

---

## System Workflow

Job Description
↓
Sentence Transformer
↓
Job Embedding
↓
Candidate Profiles
↓
Candidate Embeddings
↓
Cosine Similarity
↓
Ranking Engine
↓
Top 100 Candidates

---

## Technologies Used

| Technology            | Purpose                 |
| --------------------- | ----------------------- |
| Python                | Core implementation     |
| Google Colab          | Development environment |
| Pandas                | Data processing         |
| NumPy                 | Numerical computations  |
| Sentence Transformers | Embedding generation    |
| all-MiniLM-L6-v2      | Semantic representation |
| Cosine Similarity     | Ranking mechanism       |
| JSONL                 | Dataset format          |
| CSV                   | Submission generation   |

---

## Dataset Statistics

* Total candidates: **100,000**
* Filtered candidates: **21,760**
* Final output: **Top 100 ranked candidates**

---

## Features

* Semantic profile understanding
* Efficient candidate retrieval
* Lightweight architecture
* Batch processing support
* Scalable ranking pipeline
* CPU-friendly implementation

---

## Future Improvements

* Hybrid Retrieval (BM25 + Semantic Search)
* FAISS Vector Database
* Cross-Encoder Re-ranking
* Learning-to-Rank Models
* Behavioral Signal Integration
* Explainable AI-based recommendations

---

## Repository Structure

```
├──India_Run_Hack_2.ipynb
├── submission.csv
├── README.md

```

---

## Results

* Successfully generated ranked candidate recommendations.
* Produced a valid submission file.
* Achieved efficient processing using Sentence Transformers and semantic similarity.

---

## Author

**Riya Shinde**

Computer Engineering Student



---

## License

This project is intended for educational and hackathon purposes.
