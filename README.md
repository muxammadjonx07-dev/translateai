# 🌍 Bidirectional Uzbek–English Neural Machine Translation

![Python](https://img.shields.io/badge/Python-3.11-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.x-red)
![Transformers](https://img.shields.io/badge/HuggingFace-Transformers-yellow)
![License](https://img.shields.io/badge/License-MIT-green)

## Project Overview

This project is an AI/ML Capstone focused on developing a Bidirectional Neural Machine Translation (NMT) system between Uzbek and English.

The system enables high-quality translation in both directions:

- Uzbek → English
- English → Uzbek

The solution is designed primarily for:

- Foreign tourists visiting Uzbekistan
- University students
- Educational purposes
- Everyday communication

---

## Business Problem

Existing commercial translation systems often provide inconsistent translations for Uzbek due to the limited amount of high-quality parallel training data.

This project aims to improve translation quality by fine-tuning a multilingual transformer model using publicly available Uzbek-English sentence pairs.

---

## Objectives

- Build an end-to-end Neural Machine Translation system
- Fine-tune a pretrained multilingual model
- Evaluate translation quality using BLEU and chrF
- Develop a simple inference interface
- Create a reproducible ML pipeline

---

# Project Structure

```
uzbek-english-nmt
│
├── app/
├── data/
│   ├── raw/
│   └── processed/
├── docs/
├── models/
├── notebooks/
├── results/
├── src/
├── tests/
│
├── README.md
├── requirements.txt
├── environment.yml
├── config.yaml
├── .gitignore
└── LICENSE
```

---

# Dataset

The project uses publicly available parallel corpora.

Main sources:

- OPUS-100
- Wikipedia
- Public Uzbek-English text corpora

Sentence pairs consist of:

```
English sentence
↓

Corresponding Uzbek translation
```

---

# Model

Baseline:

```
facebook/nllb-200-distilled-600M
```

Training approach:

- Transfer Learning
- Fine-tuning
- Seq2Seq Learning

---

# Evaluation

Metrics:

- BLEU
- chrF

Additional evaluation:

- Human qualitative assessment
- Tourist phrases
- Academic sentences

---

# Technologies

- Python
- PyTorch
- HuggingFace Transformers
- Datasets
- SentencePiece
- Gradio

---

# Installation

Clone repository

```bash
git clone https://github.com/YOUR_USERNAME/uzbek-english-nmt.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# Training

```bash
python src/train.py
```

---

# Evaluation

```bash
python src/evaluate.py
```

---

# Inference

```bash
python src/inference.py
```

---

# Web Demo

```bash
python app/app.py
```

---

# Future Improvements

- Cyrillic ↔ Latin normalization
- Speech-to-text support
- Mobile application
- Better domain adaptation
- Larger training dataset

---

# Author

Muhammadjon Xalimov

INHA University in Tashkent

AI/ML Fundamentals Capstone

2026
