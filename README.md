# 📊 Comparative Analysis of Cloud-based GPT API and Local LLaMA for Educational Feedback Generation

This repository presents a comprehensive experimental study comparing **cloud-based Large Language Models (LLMs)** accessed via **GPT API** with **locally deployed LLaMA models (via Ollama)** for **automated feedback generation in higher education**.

The study evaluates how different **prompting strategies** and **persona-based instructions** influence feedback quality, measured using **multiple NLP evaluation metrics**.

---

## 🎯 Research Objectives

This project aims to:

- Compare **cloud LLMs (GPT API)** vs **local LLMs (LLaMA)** in educational feedback tasks
- Analyze the impact of **prompting strategies**:
  - Zero-shot
  - One-shot
  - Few-shot
  - Chain-of-Thought (CoT)
- Evaluate feedback quality using **multi-metric evaluation**
- Assess **persona-based prompting**:
  - Base assistant
  - Lecturer (Dosen)
  - Subject-matter expert (Ahli)
- Provide empirical insights for **AI-assisted learning and assessment**

---

## 🧠 Educational Domains

Experiments were conducted on two university-level courses:

1. **Sistem Cerdas (Artificial Intelligence)**
2. **Metodologi Penelitian dan Penulisan Ilmiah (Research Methodology)**

Each domain uses **domain-specific prompts and reference feedback**.

---

## 🤖 Models Compared

### Cloud-based LLM
- **GPT API** (e.g. GPT-4o-mini)
- Accessed via OpenAI API
- Hosted and managed externally

### Local LLM
- **LLaMA 3.1**
- Deployed locally using **Ollama**
- No API cost, full data privacy

---

## 🧪 Prompting Strategies

| Strategy | Description |
|--------|-------------|
| Zero-shot | Direct instruction without examples |
| One-shot | Single example provided |
| Few-shot | Multiple examples provided |
| CoT | Chain-of-Thought reasoning guidance |

---

## 👤 Persona-Based Prompting

Each prompt is conditioned using one of the following personas:

- **Base** – Neutral AI assistant
- **Dosen** – Lecturer providing pedagogical feedback
- **Ahli** – Subject-matter expert with academic rigor

---

## 📏 Evaluation Metrics (Multi-Metric Analysis)

Generated feedback is evaluated against reference feedback using:

- **BLEU** – n-gram precision
- **ROUGE-L** – longest common subsequence
- **METEOR** – semantic alignment with synonym handling
- **BERTScore (F1)** – contextual semantic similarity using transformer embeddings

This multi-metric approach ensures both **lexical and semantic quality assessment**.

---

## 📈 Analysis & Visualization

The repository includes:

- Per-strategy and per-persona performance analysis
- Boxplots and bar charts for metric distributions
- Cross-model comparisons (GPT vs LLaMA)
- Best-performing strategy–persona–model combinations

Visualizations are generated using **Matplotlib** and **Seaborn**.

---

## 🖥️ Interactive Demo

A **Gradio-based web interface** is provided to:

- Generate feedback interactively
- Compare GPT vs LLaMA outputs side-by-side
- Support both **single text input** and **batch file input (CSV/XLSX)**

> Note: Gradio runs locally and does not store widget state in notebook metadata.

---
