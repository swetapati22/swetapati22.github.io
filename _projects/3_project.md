---
layout: page
title: Enhancing Gentopia with AI Agents
description: Extending the Gentopia framework with a Currency Conversion Agent and a PDF Reader Agent for real-time exchange rates and document analysis.
img: assets/img/ai_agents2.png
importance: 3
category: fun
---

    ---
    Source Code available in the repository
    Github handle: swetapati22
    Project: Enhancing Gentopia with AI Agents
    ---

Source Code: <a href="https://github.com/swetapati22/Gentopia-Mason" target="_blank">Click here</a>


## **Overview**
This project enhances the **Gentopia-Mason framework** by developing and integrating **two AI-powered agents**:
1. **Currency Conversion Agent** – Fetches real-time exchange rates using the **Fixer.io API**.
2. **PDF Reader Agent** – Extracts text from **PDF documents hosted online**.

These agents **expand Gentopia’s capabilities**, enabling practical real-world applications in **currency conversion and document processing**.

---

## **Tech Stack**
- **Python** – Backend scripting and API integration.
- **Gentopia Framework** – Modular LLM agent development.
- **Fixer.io API** – Real-time currency exchange rates.
- **PyPDF2** – PDF text extraction.
- **HTTP Requests** – Web-based document fetching.
- **Git & GitHub** – Version control & collaboration.

---

## **1️. Currency Conversion Agent**
Added a **real-time currency exchange agent** to **Gentopia**, allowing users to fetch **live exchange rates** dynamically.

#### **How It Works**
- Retrieves **real-time currency conversion** data from **Fixer.io API**.
- Processes **user queries** dynamically to fetch the latest exchange rates.
- Ensures **up-to-date conversions** across multiple currencies.

#### **Implementation**
- Cloned the **Scholar Agent** from Gentopia’s pool.
- Customized the agent’s **configuration file** to support currency conversion.
- Integrated **Fixer.io API** for fetching real-time exchange rates.

```yaml
model_name: gpt-3.5-turbo
Plugins:
  - name: currency_conversion
target_tasks:
  - currency conversion
```

#### **Running the Currency Conversion Agent**
```bash
python assemble.py currency_conversion_agent
```
Once deployed, the agent can process **real-time currency conversion requests** efficiently.

---

## **2️. PDF Reader Agent**
Developed an agent for **reading and extracting text from PDFs hosted online**.

#### **How It Works**
- Accepts a **URL pointing to a PDF document**.
- Fetches the file using **HTTP requests**.
- Extracts and processes text using **PyPDF2**.

#### **Implementation**
- Cloned an agent template from Gentopia’s pool.
- Developed a new **PDFReader tool** that:
  - **Fetches a PDF** from a given **URL**.
  - **Extracts text** using **PyPDF2**.
  - **Handles errors** for **non-accessible or invalid PDFs**.

```yaml
model_name: gpt-3.5-turbo
Plugins:
  - name: pdf_reader
target_tasks:
  - PDF document text extraction
```

#### **Running the PDF Reader Agent**
```bash
python assemble.py pdf_reader_agent
```
The agent efficiently retrieves **text content from any public PDF** and makes it available for processing.

---

## **How to Run the Project**
#### **1. Clone the Repository**
```bash
git clone https://github.com/swetapati22/Gentopia-Mason.git
cd Gentopia-Mason
```

#### **2️. Set Up Virtual Environment**
```bash
conda create --name gentenv python=3.10
conda activate gentenv
pip install -r requirements.txt
```

#### **3️. Configure Environment Variables**
```bash
cd GentPool
touch .env
echo "OPENAI_API_KEY=<your_openai_api_key>" >> .env
```

#### **4️. Initialize and Run the Agents**
###### **Run Currency Conversion Agent**
```bash
python assemble.py currency_conversion_agent
```

###### **Run PDF Reader Agent**
```bash
python assemble.py pdf_reader_agent
```

---

## **Improvements Made**
- **Expands Gentopia’s agent framework** with **real-time currency conversion** and **document-processing tools**.
- **Integrates external APIs** (Fixer.io & PyPDF2) for practical, real-world applications.
- **Demonstrates AI’s versatility** in finance and information retrieval.

---
This **enhanced Gentopia project** bridges **LLM-powered automation** with **real-time currency conversion and document-processing solutions**.

