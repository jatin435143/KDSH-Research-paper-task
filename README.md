# KDSH 2024 – Research Paper Classification Task

This project was developed as part of the KDSH 2024 shared task. The objective was to build a two-stage classification system for research papers based on reliability and relevance.

## 🔍 Task Overview

- **Stage 1 – Publishability Classification**  
  Classify research papers as **publishable** or **non-publishable** by analyzing contextual reliability—such as explanation completeness, justification of claims, and factual consistency.

- **Stage 2 – Conference Assignment**  
  For papers classified as publishable, assign them to suitable conferences (e.g., NeurIPS) based on content semantics and writing style.

## 🧠 Approach

- **Text Preprocessing**  
  Cleaned and tokenized paper texts. Extracted key linguistic and semantic features from each document.

- **Feature Engineering**  
  - Extracted **BERT embeddings** to capture deep contextual meaning  
  - Used **POS tags** and **syntax patterns** to enrich linguistic structure  
  - Combined all features to form robust input vectors

- **Modeling**  
  Trained an **XGBoost classifier** to handle both stages of classification, with separate pipelines for publishability prediction and conference assignment.

## ✅ Evaluation

- Model performance was validated using accuracy and qualitative review.  
- Standard metrics such as Pearson correlation and RMSE were explored for insight but not used as final reporting metrics due to limited ground truth.

## 🔈 Additional Work

- **Speech-to-Text Module**  
  Transcribed **444 diverse audio clips** using **Whisper ASR**, improving transcript quality by approximately **40%** compared to baseline outputs.

---


