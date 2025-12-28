# Medical Text Preprocessing & Normalization

## Overview
This project is part of a **cloud-based LLM system for medical record summarization**.  
It focuses on **cleaning and normalizing medical text** so it is ready for downstream AI/NLP tasks (NER, UMLS linking, embeddings, summarization).

Preprocessing is the first step in your medical NLP pipeline and ensures data quality, consistency, and model readiness.

---

## Dataset
- **Source:** [TimSchopf/medical_abstracts](https://huggingface.co/datasets/TimSchopf/medical_abstracts)  
- **Size:** ~14,000 medical abstracts  
- **Split:** 80% train, 20% test  
- **Preprocessed CSVs:** saved in `data/` for reuse in downstream projects  

  Note: raw Hugging Face datasets are not included in GitHub to reduce size. You can download them directly from Hugging Face.

---

## Methodology
1. Lowercase text and remove accents  
2. Remove special characters and normalize whitespace  
3. Expand medical abbreviations (e.g., `HTN → hypertension`, `DM → diabetes mellitus`)  
4. Split dataset into **train/test sets**  

---

## Results
- Preprocessed and normalized text saved as CSV for downstream projects:  
  - `data/train_preprocessed.csv`  
  - `data/test_preprocessed.csv`  
- Example preprocessed text:
