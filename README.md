# 🇹🇷 Istanbul Data Jobs — Market Analysis

A Python-based scraper and analysis notebook that explores what skills, tools, and technologies Istanbul employers are looking for in Data Science, Data Analyst, and Machine Learning roles.

Built from real job postings scraped from **LinkedIn** and **Kariyer.net**.

---

## 🔍 What This Project Does

- Scrapes live job postings for data roles in Istanbul
- Extracts and ranks **100+ skills** across 9 categories (ML models, programming languages, cloud platforms, tools, and more)
- Breaks down skill demand **by role** — Data Scientist vs Data Analyst vs ML Engineer
- Visualizes everything with charts, heatmaps, and a word cloud

---

## 📊 Key Findings

- **Python** and **SQL** appear in the vast majority of postings across all roles
- **XGBoost** and **scikit-learn** are the most requested ML tools
- **Power BI** and **Tableau** dominate for analyst roles
- **AWS** is the leading cloud platform requested
- Time series and anomaly detection skills are increasingly common in ML Engineer postings

---

## 🛠️ Tools & Libraries

| Purpose | Libraries |
|---------|-----------|
| Scraping | `requests`, `BeautifulSoup`, `lxml` |
| Data Processing | `pandas`, `numpy` |
| Visualization | `matplotlib`, `seaborn`, `plotly`, `wordcloud` |
| Notebook | Google Colab / Jupyter |

---

## 🚀 How to Run

1. Open the notebook in Google Colab:

   (https://colab.research.google.com)

2. Install dependencies (first cell handles this automatically)

3. Run all cells — the scraper will collect fresh job postings and generate all charts

> ⏱️ Full run takes around 10–15 minutes depending on how many pages you scrape

---

## 📁 Files

```
istanbul-job-market/
│
├── istanbul_job_scraper_v2.ipynb   # Main notebook
├── README.md                       # This file
└── sample_output/
    ├── istanbul_jobs.csv           # Sample scraped jobs
    └── istanbul_skills_summary.csv # Skills frequency table
```

---

## ⚙️ Configuration

You can easily customize the scraper at the top of the notebook:

```python
SEARCH_KEYWORDS = ["data scientist", "data analyst", "machine learning engineer", ...]
LOCATION        = "Istanbul"
MAX_PAGES       = 3      # increase for more results
FETCH_DESCRIPTIONS = True  # set False for faster run
```

---

*Data scraped from LinkedIn and Kariyer.net. For educational and portfolio purposes only.*
