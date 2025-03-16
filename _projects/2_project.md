---
layout: page
title: YouTube Global Statistics Analytics
description: A Data Visualization, interactive web application project to analyze global YouTube trends enabling dynamic exploration through interactive insights.
img: assets/img/preswald_cover_analytics.gif
importance: 2
category: work
giscus_comments: true
---
    ---
    Source Code available in the repository
    Github handle: swetapati22
    Project: YouTube Global Statistics Analytics
    Repository: https://github.com/swetapati22/youtube_statistics_analytics_dashboard
    Dataset: https://www.kaggle.com/datasets/nelgiriyewithana/global-youtube-statistics-2023?resource=download
    Dashboard Preview Link: https://my-example-project-514006-3h0rzgww-ndjz2ws6la-ue.a.run.app 
    Demo Video Link: https://drive.google.com/file/d/1dIltYoPJXD8v64u2FJ1dohb0a2Vnw4o0/view?usp=sharing 
    ---

## **Overview**
**A Data Visualization, interactive web application project using Plotly, Preswald, Python, and Pandas** to analyze **global YouTube trends** across **categories, creators, and countries**. Enabling **dynamic exploration** through **interactive insights** using **Global YouTube Statistics 2023** dataset.

The application features **six interactive visualizations** and **a dynamic slider filter** to enhance interactivity.

---
## **Tech Stack**
- **Preswald** – For interactive UI & visualization.
- **Pandas** – Data manipulation & filtering.
- **Plotly** – Graphical visualizations (bar charts, line graphs, maps, heatmaps).
- **Python** – Backend scripting.
- **Git & GitHub** – Version control & collaboration.

---
## **Dataset Details**
- **Dataset:** Global YouTube Statistics 2023:   
- **Dataset Source:** Kaggle  

---
## **Global Filter - Slider for Views Threshold**
Before visualizing data, the app includes a **slider filter** that allows users to **set a minimum threshold** for video views.  
This ensures dynamic exploration based on user preferences.

```python
views_threshold = slider("Minimum Views (Converted to Billion)", min_val=0, max_val=max_views, default=0.5)
```
Once a threshold is selected, the **six different visualizations** are displayed.

---
## **Visualizations**

### **1. Views by Category (Bar Chart)**
**Graph Type:** 📊 **Bar Chart (Categorical Comparison)**  
- Displays **total YouTube video views** for different **content categories**.
- Users can **identify top-performing categories**.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p1.png" title="Views by Category" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Analytical Insights:**  
- **Most popular category**: **Music**, accumulating **2928.88 billion** views, highlighting its **massive audience engagement**.  
- **Least popular categories**: **Travel & Events, Movies, Nonprofits & Activism** – indicating **niche audiences** with smaller but dedicated followings.

---

### **2. Top YouTubers by Views (Bar Chart)**
**Graph Type:** 📊 **Bar Chart (Ranked List)**  
- Highlights **top YouTubers** based on **total video views**.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p2.png" title="Top YouTubers by Views" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Analytical Insights:**   
- **Most-watched YouTuber**: **T-Series**, amassing **228.00 billion** views, demonstrating a **strong and consistent audience reach**.  
- The distribution of views indicates **category dominance**, where **Entertainment, Music, and Gaming** outperform niche educational or specialized content.

---

### **3. YouTube Views by Country (Choropleth Map)**
**Graph Type:** 🌍 **Choropleth Map (Geographical Data Representation)**  
- Displays **YouTube viewership per country**.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p3.png" title="YouTube Views by Country" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Analytical Insights:**  
- **Country with highest YouTube engagement**: **United States**, leading with **3557.44 billion** views, showcasing its **massive audience and content consumption**.  
- **Lowest engagement regions**: **Peru, Finland, Andorra** – potentially due to **smaller population sizes, lower internet penetration, or niche content interests**.

---

### **4. Category Trends Across Countries (Heatmap)**
**Graph Type:** 🔥 **Heatmap (Regional Comparison)**  
- Illustrates how **YouTube content categories** perform across **different countries**.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p4.png" title="Category Trends Across Countries" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Analytical Insights:**  
- **United States** has the **highest YouTube views globally** with **3557.44 billion** views, with **Music** as the **most-watched category**, accumulating **1012.12 billion** views.  
- **Least-watched categories globally**: **Travel & Events, Movies, Nonprofits & Activism** – suggesting these categories **cater to niche audiences rather than mass engagement**.

---

### **5. Trending YouTubers (Last 30 Days) (Line Chart)**
**Graph Type:** 📈 **Line Chart (Time Series Analysis)**  
- Tracks **YouTube creators trending in the last 30 days**.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p5.png" title="Trending YouTubers" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Analytical Insights:**   
- **Most trending YouTuber**: **ıııııııı KIMPRO**, accumulating **3.4 billion** views in the past **30 days**.  
- **Largest drop in engagement**: **ArianaGrandeVevo**, indicating a **potential decline in engagement** or **reduced content uploads**.

---

### **6. Subscribers vs Uploads Growth (Multi-Line Chart)**
**Graph Type:** 📈 **Multi-Line Chart (Trend Comparison)**  
- Analyzes the relationship between **content uploads & subscriber growth**.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/preswald_p6.png" title="Subscribers vs Uploads Growth" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Analytical Insights:**  
- **Category with highest subscriber growth**: **Film & Animation**, reaching **86.90 million** subscribers, demonstrating **strong audience engagement**.  
- **Category with lowest subscriber growth**: **Travel & Events**, with only **12.50 million** subscribers, suggesting that **more uploads do not necessarily translate to higher subscriber gain**.  
- **Not all categories grow equally** – **quality content matters more than quantity** in some cases.

---
## **How to Run the Project**
### **1. Install Preswald**
```bash
pip install preswald
```

### **2. Initialize Project**
```bash
preswald init my_example_project
cd my_example_project
```

### **3. Download Dataset**
Place the dataset in the **data/** folder inside the project.

### **4. Run Locally**
```bash
preswald run
```

### **5. Deploy to Structured Cloud**
```bash
preswald deploy --target structured --github <your-github-username> --api-key <structured-api-key> hello.py
```
Replace `<your-github-username>` and `<structured-api-key>` with your credentials.

---
## **Major Takeaways:**
- **YouTube trends vary significantly** by category, creator, and region.  
- **Trending creators fluctuate frequently**, requiring continuous audience engagement.  
- **Content quality > Upload quantity** for some categories.  

---
This **interactive dashboard** provides valuable insights for **content creators, analysts, and marketers** to understand **global YouTube trends** dynamically.
