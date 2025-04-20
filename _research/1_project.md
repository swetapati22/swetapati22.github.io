---
layout: page
title: Instruction-Tuned LLMs for Event Extraction
importance: 1
description: Research on enhancing event extraction using instruction-tuned large language models (LLMs), optimizing annotation guidelines, and improving fine-tuning techniques for NLP tasks.
img: assets/img/EE_Research.gif
category: Machine Learning and AI
---
    ---
    Research conducted at George Mason University (GMU) - Natural Language Processing Lab
    Research Supervisor: Professor Ziyu Yao
    Conference Submission: ACL 2025
    ---

---
## **📜 Research Paper & Resources**
- **ACL 2025 Submission**: Source Code: <a href="https://arxiv.org/abs/2502.16377" target="_blank">Instruction-Tuning LLMs for Event Extraction with Annotation Guidelines</a> (In-Review)
- **Research Institution**: George Mason University (GMU), NLP Lab 
- **Focus Area**: **Event Extraction**, **Instruction-Tuned LLMs**, **Annotation Guideline Generation**
- **Code Repository**: *(Coming Soon!)*
- **Dataset & Annotation Guidelines**: *(Coming Soon!)*

---

## **🛠 Tech Stack & Tools**
- **Machine Learning & NLP**: LLaMA-3.1, Hugging Face Transformers, PyTorch, LoRA Fine-Tuning, Unsloth, Quantization
- **Data Processing**: JSON, Python (Pandas, Numpy)
- **GPU Resources**: HPC, CUDA
- **Evaluation Metrics**: Precision, Recall, F1-score

---

## **📖 Research Overview**

This research explores the **enhancement of event extraction (EE) tasks** by leveraging **instruction-tuned large language models (LLMs)**. Traditional event extraction models struggle with **limited training data, ambiguous event definitions, and scalability**. To address these challenges, our approach:

- **Synthesizes annotation guidelines** for **500+ event types** and **4000+ argument structures**  
- **Fine-tunes LLaMA-3.1 8B** using **LoRA and structured regularization techniques**  
- **Develops an evaluation framework** for optimizing inference speed and cost efficiency  
- **Reduces hallucinations** by transforming text-based evaluations into **code-based prompt optimization**  

This work aims to improve **F1-score performance** on **event extraction tasks** and **enhance the reliability** of LLM-generated event predictions.

---

## **📊 Major Contributions**

### **1. Annotation Guideline Optimization**
- Developed a structured framework for creating **high-quality event extraction annotation guidelines**.
- Synthesized event schema covering **500+ event types** and **4000+ argument structures** using **GPT-4o**.

### **2. LLM Fine-Tuning & Optimization**
- Implemented **Low-Rank Adaptation (LoRA)** for **fine-tuning LLaMA-3.1 8B** on event extraction tasks using **unsloth** library.
- Improved **model efficiency** using **structured regularization** techniques.

### **3. Cost-Effective & Low-Latency Inference Pipelines**
- Designed a **scalable NLP pipeline** using **GPU-optimized environments**.
- Optimized inference by **reducing hallucination through implicit prompt engineering** guided by annotations for each event type.

### **4. Performance Improvement**
- Achieved a **10% increase in F1-score** compared to traditional event extraction baselines.
- Enhanced the **generalization ability** of instruction-tuned LLMs across multiple datasets.

---

## **Future Work & Applications**
**Expanding dataset coverage** to include **multi-domain event extraction** tasks  
**Exploring multimodal event extraction** by integrating **text, images, and video content**  

---

*For collaboration or inquiries, feel free to reach out via [LinkedIn](https://www.linkedin.com/in/sweta-pati/) or [Email](mailto:spati@gmu.edu).*

