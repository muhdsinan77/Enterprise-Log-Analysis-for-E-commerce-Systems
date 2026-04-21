# Enterprise Log Analysis for E-Commerce Systems

## Project Overview

This project analyses real web server logs from an online shopping store to understand user behaviour, detect traffic patterns and identify anomalies using Python-based data science tools. The system reads raw log files line by line, extracts timestamps using Regular Expressions, organises data using Pandas, generates visualisation charts using Matplotlib, and detects unusual traffic hours using Scikit-learn's Isolation Forest algorithm.

---

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data cleaning and organisation |
| Matplotlib | Data visualisation (bar, line, pie charts) |
| Scikit-learn | Machine learning — anomaly detection |
| Regex (re module) | Timestamp extraction from log files |
| Jupyter Notebook | Development and execution environment |

---

## Dataset

**Source:** Online Shopping Store — Web Server Logs  
**Repository:** Harvard Dataverse  
**Link:** https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/3QBYB5

The dataset contains real Nginx server access logs from an actual e-commerce store. Three log files are used — `browse`, `product` and `basket` — each recording timestamped user activity.

---

## Project Structure

```
log-analysis-ecommerce/
├── log_analysis.ipynb       # Main Jupyter Notebook
├── README.md                # Project documentation
├── dataset/
│   ├── browse               # Browse activity log
│   ├── product              # Product view log
│   └── basket               # Basket addition log
├── documents/
│   ├── HLD_Muhammed_Sinan.docx
│   └── LLD_Muhammed_Sinan.docx
└── outputs/
    ├── bar_chart.png
    ├── line_chart.png
    ├── pie_chart.png
    └── anomaly_chart.png
```

---

## How to Run

**Step 1 — Install required libraries**
```
pip install pandas matplotlib scikit-learn
```

**Step 2 — Download the dataset**

Download the log files from Harvard Dataverse (link above) and place them in the `dataset/` folder.

**Step 3 — Open and run the notebook**
```
jupyter notebook log_analysis.ipynb
```

Run all cells from top to bottom using **Cell > Run All**.

---

## Key Findings

- **Total Browse Events:** 5,378,843
- **Total Product Events:** 13,779,768
- **Total Basket Events:** 632,326
- **Conversion Rate:** 11.76%
- **Peak Browse Hour:** 11 AM
- **Anomalous Hours Detected:** 10 AM and 11 AM
- **Activity Share:** Product 69.6% | Browse 27.2% | Basket 3.2%

---

## Output Charts

| Chart | Description |
|---|---|
| Bar Chart | Browse, product and basket event counts per hour |
| Line Chart | Activity trend over the course of the day |
| Pie Chart | Overall percentage share of each activity type |
| Anomaly Detection | Hours flagged as anomalous by Isolation Forest |

---

## Documents

| Document | Description |
|---|---|
| HLD | High Level Design — system architecture and design |
| LLD | Low Level Design — module-level code design |

---

## Author

**Name:** Muhammed Sinan  
**Institution:** Yenepoya Institute of Arts, Science, Commerce and Management  
**Programme:** BCA — Final Year Project  
**Industry Mentor:** Sumit Kumar Shukla  
**College Guide:** Raksha Adyanthaya  
**Academic Year:** 2025–2026
