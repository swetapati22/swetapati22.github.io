---
layout: page
title: Spotify 2023 Streaming Analysis
description: Exploring the most streamed artists, songs, and industry trends of 2023 through interactive data visualization.
img: assets/img/Spotify_analysis.jpeg
importance: 1
category: fun
---

    ---
    Source Code available in the repository
    Github handle: saileshdwivedy30
    Project: Spotify 2023 Streaming Analysis
    Deployed App: https://my-example-project-719255-kngkr5dp-ndjz2ws6la-ue.a.run.app/
    Demo Video: https://drive.google.com/file/d/13TnESRwxw4Eew5h-zCw-aM1MxVO8Ncld/view?usp=sharing
    Dataset Link: https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023/data    
    ---

## **Overview**
The **Spotify 2023 Streaming Analysis App** is an **interactive data visualization platform** that explores **top streamed songs, artists, and industry trends**. It enables **music analysts, data enthusiasts, and industry professionals** to analyze how **song characteristics, playlist placements, and seasonal trends** influence streaming performance.

For a detailed walkthrough, please check out the **demo video** linked above.

---

## **Tech Stack**
- **Python** – Backend scripting and data processing.
- **Pandas & NumPy** – Data analysis and manipulation.
- **Plotly & Seaborn** – Interactive visualizations and charts.
- **Preswald** – UI framework for interactive dashboards.
- **Flask** – Backend for web app deployment.
- **Git & GitHub** – Version control and project collaboration.

---

## **Dataset Overview**
The project utilizes the **Most Streamed Spotify Songs 2023** dataset from **Kaggle** (linked above), containing:
- **Top streamed songs & artists**
- **Streaming counts and ranking trends**
- **Song attributes** (BPM, energy, danceability, valence, etc.)
- **Playlist placements across streaming platforms**

---
## **Features & Insights**
This app provides **interactive visualizations and insights** into the world of **Spotify streaming trends**:

### **1️. Top Artists by Total Streams**
- **Bar chart** showcasing **most streamed artists globally**.
- Analyze **trends in artist dominance** over the year.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p3.png" title="YouTube Views by Country" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### **2️. Most Streamed Songs**
- **Interactive ranking chart** of viral hits and long-lasting chart-toppers.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p3.png" title="YouTube Views by Country" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### **3️. Impact of BPM on Song Popularity**
- **Scatter plot** analyzing the correlation between **tempo (BPM) and total streams**.
- Do **high-energy songs** perform better, or do **slow-tempo ballads** dominate?

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p3.png" title="YouTube Views by Country" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### **4️. Trends in Song Releases Over the Years**
- **Line chart** tracking **evolution of song releases** over time.
- Assess **the impact of streaming platforms** on **independent artists**.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p3.png" title="YouTube Views by Country" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### **5️. How Do Song Characteristics Affect Popularity?**
- **Energy vs. Streams, Danceability vs. Streams (Scatter Plots)**
- **Happiness (Valence) Analysis using Box Plot**
- Identifying **traits that define viral hits**.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p3.png" title="YouTube Views by Country" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p3.png" title="YouTube Views by Country" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### **6️. Influence of Playlist Placements on Streams**
- **Comparison of playlist placements** across **Spotify, Apple Music, and Deezer**.
- **Scatter plot:** Does **playlist exposure** significantly boost **streaming numbers**?

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p3.png" title="YouTube Views by Country" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### **7️. Seasonal Trends in Song Releases & Streaming**
- **Monthly trends in song releases and streaming activity**.
- Identify **peak months** for **new music releases** and **streaming surges**.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p3.png" title="YouTube Views by Country" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### **8️. Key & Mode Distribution of Popular Songs**
- **Bar chart** for **most common musical keys**.
- **Pie chart** analyzing **major vs. minor modes** in **top songs**.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p3.png" title="YouTube Views by Country" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p3.png" title="YouTube Views by Country" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

---

## **How to Run the Project**
#### **1. Clone the Repository**
```bash
git clone https://github.com/saileshdwivedy30/spotify_2023_analysis.git
cd spotify_2023_analysis
```

#### **2⃣. Set Up Virtual Environment**
```bash
pip install -r requirements.txt
```

#### **3⃣. Run the App Locally**
```bash
preswald run
```

#### **4⃣. Deploy the App**
```bash
preswald deploy --target structured --github <your-github-username> --api-key <structured-api-key> app.py
```
Replace `<your-github-username>` and `<structured-api-key>` with your credentials.

---

## **Key Takeaways**
- **Data-driven insights** into **Spotify’s 2023 streaming trends**.
- **Interactive visualizations** to explore **artist & song performance**.
- **Seasonal and playlist-driven impact** on **streaming numbers**.
- **Deployable web app** with **easy-to-use filtering & analysis**.

---
This **interactive dashboard** is designed for **music analysts, content creators, and industry professionals** to explore **Spotify’s 2023 streaming trends dynamically**.