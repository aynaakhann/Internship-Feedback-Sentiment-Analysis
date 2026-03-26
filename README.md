# Internship Feedback Sentiment Analysis

> An end-to-end Natural Language Processing (NLP) project that classifies internship feedback as \*\*Positive\*\*, \*\*Neutral\*\*, or \*\*Negative\*\* using Python and VADER Sentiment Analysis.

\---

## Overview

This project was completed as part of a **Data Analyst Internship at** [**Internee.pk**](https://internee.pk). The goal was to evaluate the emotional tone of intern feedback collected from multiple sources — surveys, comments, and social media — and extract meaningful insights to help improve the internship experience.

Sentiment analysis is one of the most widely used applications of Natural Language Processing (NLP) in the real world. Companies use it to analyze customer reviews, employee feedback, social media mentions, and more. This project simulates exactly that use case in a professional setting.

\---

## Objectives

* ✅ Build a structured dataset of **120+ intern feedback entries** from multiple sources
* ✅ Perform sentiment analysis using **Python (NLTK — VADER)**
* ✅ Classify each feedback as **Positive**, **Neutral**, or **Negative**
* ✅ Visualize results using a **multi-panel professional dashboard**
* ✅ Export results to CSV for reporting and further analysis

\---

## Dataset

The dataset was **custom-built** for this project, simulating real-world intern feedback across multiple touchpoints.

|Column|Description|
|-|-|
|`feedback\_id`|Unique ID for each feedback entry|
|`feedback\_text`|The actual feedback written by the intern|
|`source`|Where the feedback came from (Survey / Comment / Social Media)|
|`intern\_department`|Department the intern belonged to|
|`internship\_month`|Month the feedback was submitted|

**Dataset Stats:**

* Total Entries: **120 rows**
* Departments covered: Data Science, Software Engineering, Marketing, Finance, HR
* Sources: Survey, Comment, Social Media
* Months: January, February, March

\---

## Tech Stack

|Tool|Purpose|
|-|-|
|**Python 3.8+**|Core programming language|
|**NLTK (VADER)**|Sentiment scoring and classification|
|**Pandas**|Data loading, manipulation, and export|
|**Matplotlib**|Chart creation and dashboard layout|
|**Seaborn**|Enhanced chart aesthetics|
|**Google Colab**|Cloud-based notebook environment|

\---

## Project Structure

```
internship-feedback-sentiment-analysis/
│
├── Sentiment\_Analysis.ipynb       # Main Google Colab notebook
├── internship\_feedback.csv        # Raw dataset (120 rows)
├── feedback\_results\_final.csv     # Output dataset with sentiment labels \& scores
├── sentiment\_dashboard.png        # 4-panel visualization dashboard
├── score\_distribution.png         # VADER compound score histogram
└── README.md                      # Project documentation (you are here)
```

\---

## How to Run

### Option 1 — Google Colab (Recommended)

1. Open [Google Colab](https://colab.research.google.com)
2. Click **File → Upload Notebook** and upload `Sentiment\_Analysis.ipynb`
3. Upload `internship\_feedback.csv` using the 📁 sidebar
4. Click **Runtime → Run All**
5. Results and charts will generate automatically

### Option 2 — Run Locally

**1. Clone this repository**

```bash
git clone https://github.com/YOUR\_USERNAME/internship-feedback-sentiment-analysis.git
cd internship-feedback-sentiment-analysis
```

**2. Install dependencies**

```bash
pip install nltk pandas matplotlib seaborn
```

**3. Run the notebook**

```bash
jupyter notebook Sentiment\_Analysis.ipynb
```

\---

## Results \& Visualizations

### Sentiment Breakdown

|Sentiment|Count|Percentage|
|-|-|-|
|😊 Positive|\~60|\~50%|
|😐 Neutral|\~22|\~18%|
|😞 Negative|\~38|\~32%|

> \*Exact numbers depend on VADER scoring. Run the notebook to see your results.\*

### Dashboard Preview

The project generates a **4-panel visual dashboard** including:

* **Pie Chart** — Overall sentiment distribution
* **Bar Chart** — Sentiment count with value labels
* **Grouped Bar Chart** — Sentiment breakdown by department
* **Grouped Bar Chart** — Sentiment breakdown by feedback source

And a separate **histogram** showing the distribution of VADER compound scores across all 120 feedback entries.

\---

## Key Learnings

* How **VADER (Valence Aware Dictionary and sEntiment Reasoner)** works and why it is well-suited for short social-media-style text
* The importance of **compound scores** and how thresholds (`≥ 0.05` / `≤ -0.05`) define sentiment classes
* How to build a **complete NLP pipeline** from raw data to visual output
* How to structure a data science project professionally for portfolio presentation
* Real-world value of sentiment analysis in **HR, product feedback, and customer experience** domains

\---

## Author

**Ayna Khan**
Data Analyst Intern — Internee.pk


