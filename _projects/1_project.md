---
layout: page
title: Implementing Authentic Counterhate Arguments
description: Reproducing and extending the EMNLP '23 study on counterhate arguments for online hate speech.
img: assets/img/counter_hate_project1.png
importance: 1
category: work
related_publications: true
---

## Overview

In this project, we **replicate and extend** the EMNLP 2023 paper **"Finding Authentic Counterhate Arguments: A Case Study with Public Figures"** by **Albanyan, Hassan, and Blanco**. This study focuses on identifying **authentic counterhate arguments** that effectively counter online **hate speech** targeted at specific individuals.

This work is part of the **"Reproducibility Challenges in Research Papers"** initiative and has been carefully documented in our Reproducibility Study Report by **Sweta Pati and Swabhi Papneja**.

Inorder to have a better understanding of our work please go through a carefully prepared Presentation.
---

## Project Objective

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/objective_box.png" title="Project Objective" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Objective:** To identify **authentic counterhate arguments** that directly refute the claims made in **hateful tweets** towards specific individuals. Counterhate responses should be **logical, fact-based, and effective** in deconstructing hateful rhetoric.

### What is Hate Speech?  
> "_A hateful speech, as per Twitter guidelines, includes any implicit or explicit tweet that attacks an individual’s **gender, religion, race, ideology, or social class**._"

### What is Counterhate?  
> "_Counterhate is a direct response that refutes hate speech. An **authentic counterhate argument** is a **fact-based** response that includes logical reasoning, testimonials, or statistical evidence._"

---

## Dataset Overview

Our dataset is derived from **hateful tweets** directed at **50 individuals**. It includes:
- **250 hateful tweets**
- **2500 articles**
- **54,816 paragraphs** (collected as supporting evidence)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/counter_hate_dataset_stats.png" title="Dataset Composition" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
---

## Approach & Methodology

To ensure a structured analysis, we break down the workflow into **four key stages**:

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/counter_hate_approach.png" title="Methodology Workflow" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### ** Data Preparation**
- Loads raw tweets, paragraphs, and articles.
- Cleans and tokenizes text using **RoBERTa** (for paragraphs) and **Longformer** (for articles).
- Splits into **training, validation, and test sets**.

### ** Model Training**
- **Fine-tunes transformers-based models** on the dataset.
- Implements **Adaptive Learning Rate Scheduling** with **AdamW optimizer**.
- Trains using a **classification loss function**.

### ** Model Evaluation**
- Evaluates on **Precision, Recall, and F1-score**.
- Compares against **published results**.

### ** Error Analysis & Interpretability**
- **Identifies misclassified samples** to analyze weaknesses.
- Generates **histograms** to visualize text characteristics.
- **Improves generalizability** via error correction.

---

## Experiments & Results

### **Dataset Splitting & Model Performance**
The dataset is divided into **article-level** and **paragraph-level** experiments. We compare our model’s **precision, recall, and F1-score** against the original paper.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/Counterhate_Arguments_result.png" title="Results Table" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Our model achieves **comparable performance** to the original implementation.

---

## 🚀 How to Run the Project

### **Clone the Repository**
```sh
git clone https://github.com/swetapati22/Counterhate_Arguments.git
```

### **Navigate to the Project Directory**
```sh
cd Counterhate_Arguments
```

### **Install Dependencies**
```sh
pip install -r requirements.txt
```

### **Data Preparation**
```sh
python prepare_data.py --csv-file <path_to_csv_file> --level <level> --output-dir <output_directory>
```

### **Train the Model**
```sh
python train.py --data-dir <processed_data_path> --level <level> --output-dir <output_path>
```

### **Evaluate the Model**
```sh
python test.py --data-dir <processed_data_path> --trained-model-dir <trained_model_path> --output-dir <output_path>
```

### **Perform Error Analysis**
```sh
python error_analysis.py --data-dir <processed_data_path> --trained-model-dir <trained_model_path> --output-dir <output_path>
```

### **Quick Run Scripts**
Instead of running steps individually, execute:
- `article_script.sh` for **article-level** processing.
- `paragraph_script.sh` for **paragraph-level** processing.

---

## Key Takeaways

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/key_takeaways.png" title="Major Findings" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

- **Reproducibility Validated**: Our results closely align with the original research.
- **Counterhate is Crucial**: Identifying **logical, evidence-backed counterhate responses** improves **online discourse**.
- **Future Work**: Exploring **multilingual generalization** of counterhate responses.

---

## Citation

If you use this work, please cite:

```
@misc{papneja_pati_2024,
  author = {Papneja, S. and Pati, S.},
  title = {Implementing Authentic Counterhate Arguments},
  year = {2024},
  url = {https://github.com/swetapati22/Counterhate_Arguments},
  note = {GitHub Repository}
}
```

