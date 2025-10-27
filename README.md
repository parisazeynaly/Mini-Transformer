# Mini-Transformer

A lightweight implementation of the Transformer architecture (1–5M parameters) designed for **two tasks** within a single project:
- **Language Modeling (LM)**: next-token prediction with Perplexity evaluation  
- **Text Classification (CLF)**: sequence classification (e.g., sentiment analysis)

 **Goal:** Build a small, interpretable, and efficient Transformer model that can run on standard GPU/CPU hardware, with clean code and reproducible results.

---

## ✨ Features
- Shared architecture with two output heads (`task="lm"` or `task="clf"`)  
- Compact design: 2–4 Transformer blocks, 128–256 hidden dimension, 2–4 attention heads  
- Supports BPE/SentencePiece tokenization (8k–16k vocabulary)  
- Training scripts for both LM and classification tasks  
- Evaluation metrics: **Perplexity (LM)**, **Accuracy/F1 (CLF)**  
- Demo inference script for generating text or predicting labels  

---

## 📂 Project Structure

mini-transformer/
├─ data/ 
├─ tokenizer/ 
├─ src/
│ ├─ model.py 
│ ├─ train_lm.py 
│ ├─ train_clf.py 
│ └─ infer.py 
├─ notebooks/ 
├─ tests/
└─ README.md 
