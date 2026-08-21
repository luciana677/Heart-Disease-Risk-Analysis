# ❤️ Heart Disease Risk Analysis

An exploratory data analysis and Power BI project investigating patient characteristics and clinical factors associated with heart disease, with the goal of identifying patterns that can support better health-risk understanding.

---

📌 Project Type
- Exploratory Data Analysis (EDA)
- Data Cleaning / Wrangling
- Dashboard / Data Visualization
- End-to-End Analytics Project

---

📑 Table of Contents

1. [Project Overview](#1-project-overview)
2. [Objectives](#2-objectives)
3. [Project Scope & Tools](#3-project-scope--tools)
4. [Repository Structure](#4-repository-structure)
5. [Data Workflow](#5-data-workflow)
6. [Dataset Overview](#6-dataset-overview)
7. [Analysis & Metrics](#7-analysis--metrics)
8. [Key Insights](#8-key-insights)
9. [Recommendations](#9-recommendations)
10. [Assumptions & Limitations](#10-assumptions--limitations)
11. [Future Enhancements](#11-future-enhancements)
12. [Dashboard](#12-dashboard)
13. [Deliverables](#13-deliverables)
14. [Author](#14-author)

---

1. Project Overview

Context

Heart disease remains an important health concern, and understanding patterns within patient data can help identify characteristics associated with increased cardiovascular risk.

Problem Statement

The objective of this project was to explore a heart disease dataset and determine how demographic and clinical factors vary between patients with and without heart disease.

Approach

The project involved data cleaning, exploratory data analysis, statistical and visual comparisons, and the development of an interactive Power BI dashboard. Key variables examined included age, gender, chest pain type, blood pressure, cholesterol, maximum heart rate, exercise-induced angina, fasting blood sugar, resting ECG, and other clinical indicators.

Outcome

The analysis produced a cleaned dataset, exploratory findings, and an interactive Power BI dashboard highlighting the distribution of heart disease and relationships between heart disease status and selected patient characteristics.

---

2. Objectives

- Primary Objective: Identify patterns and clinical factors associated with heart disease within the dataset.
- Secondary Objective 1: Clean and prepare the dataset for reliable analysis and visualization.
- Secondary Objective 2: Compare demographic and clinical characteristics between patients with and without heart disease.
- Secondary Objective 3: Develop an interactive Power BI dashboard that communicates the findings clearly.
- Secondary Objective 4: Translate the analysis into practical, data-driven insights.

---

3. Project Scope & Tools

Scope

Dimension| Details
In Scope| Patient demographics, clinical measurements, heart disease status, exploratory analysis and dashboard visualization
Out of Scope| Clinical diagnosis, treatment recommendations, or individual patient risk prediction
Dataset Size| 920 patient records
Granularity| One row represents an individual patient
Analysis Focus| Factors associated with heart disease status

Tools & Technologies

Category| Tool(s) Used
Data Source| CSV Dataset
Data Processing| Python
Data Analysis| Python / Jupyter Notebook
Visualization| Power BI
Version Control| Git / GitHub
Documentation| Markdown

---
```
4. Repository Structure

❤️ Heart-Disease-Risk-Analysis
│
├── 📂 data
│   ├── 📂 raw
│   │   └── heart_disease.csv
│   │
│   └── 📂 processed
│       └── heart_disease_cleaned.csv
│
├── 📂 notebooks
│   └── heart_disease_analysis.ipynb
│
├── 📂 visuals
│   ├── 📂 dashboard
│   │   └── heart_disease_dashboard.png
│   │
│   └── 📂 eda
│       └── [selected EDA visuals]
│
├── 📄 .gitignore
└── 📄 README.md
```
---

5. Data Workflow
```
Raw Dataset
     ↓
Data Inspection
     ↓
Data Cleaning
     ↓
Exploratory Data Analysis
     ↓
Feature Preparation
     ↓
Power BI Visualization
     ↓
Dashboard & Insights
```
1. Data Source

The project used a heart disease dataset containing patient demographic and clinical information.

2. Data Inspection

The dataset was examined for its structure, data types, missing values, duplicate records, unusual values, and potential data-quality issues.

3. Data Cleaning

Missing values and data-quality issues were investigated and addressed before visualization. Variables including "ca", "thal", and "slope" required particular attention because of missing observations.

4. Exploratory Analysis

The analysis examined heart disease distribution and relationships between heart disease status and selected demographic and clinical variables.

5. Visualization

Key findings were transformed into interactive Power BI visuals and dashboard components.

6. Output

The final outputs include a cleaned dataset, analytical notebook, visualizations, and an interactive Power BI dashboard.

---

6. Dataset Overview

Dataset Description

The dataset contains patient-level demographic and clinical variables used to investigate patterns associated with heart disease.

| Field | Description |
|-------|-------------|
| `age` | Patient age |
| `sex` | Patient sex |
| `cp` | Chest pain type |
| `trestbps` | Resting blood pressure |
| `chol` | Serum cholesterol |
| `fbs` | Fasting blood sugar indicator |
| `restecg` | Resting electrocardiographic results |
| `thalach` | Maximum heart rate achieved |
| `exang` | Exercise-induced angina |
| `oldpeak` | ST depression induced by exercise |
| `slope` | Slope of the peak exercise ST segment |
| `ca` | Number of major vessels |
| `thal` | Thalassemia-related measurement |
| `heart_disease` | Heart disease status |

Dataset Size

- Rows: 920
- Unit of analysis: Individual patient
- Target variable: "heart_disease"

---

7. Analysis & Metrics

Analytical Approach

The analysis focused on identifying differences and patterns between patients with and without heart disease.

The following areas were investigated:

- Heart disease distribution
- Age and heart disease
- Gender and heart disease
- Chest pain type and heart disease
- Exercise-induced angina
- Fasting blood sugar
- Resting ECG
- Cholesterol
- Resting blood pressure
- Maximum heart rate
- Other available clinical indicators

Key Metrics

| Metric | Definition | Purpose |
|--------|------------|---------|
| **Heart Disease Count** | Number of patients classified with heart disease | Understand overall disease distribution |
| **Heart Disease Rate** | Patients with heart disease ÷ total patients | Measure prevalence within the dataset |
| **Average Age** | Mean patient age by heart disease status | Compare age patterns |
| **Average Cholesterol** | Mean cholesterol level by heart disease status | Examine cholesterol differences |
| **Average Max Heart Rate** | Mean maximum heart rate by heart disease status | Identify differences in exercise-related heart performance |

---

8. Key Insights

Insight 1 — Heart Disease Distribution

The dataset contains both patients with and without heart disease, allowing comparison between the two groups.

Insight 2 — Age

Heart disease generally showed a stronger presence among older patients, although the 70+ age group contained fewer observations and should therefore be interpreted cautiously.

Insight 3 — Chest Pain

Chest pain type showed noticeable differences across heart disease groups, making it one of the important variables explored in the analysis.

Insight 4 — Exercise-Induced Angina

Exercise-induced angina showed a notable relationship with heart disease status, suggesting that exercise-related symptoms are an important variable to examine alongside other clinical factors.

Insight 5 — Cholesterol

Cholesterol levels showed differences between patients with and without heart disease. The dataset also contained suspicious zero cholesterol values, highlighting the importance of data-quality checks before drawing conclusions from the variable.

---

9. Recommendations

«These recommendations are intended as data-analysis recommendations, not medical advice.»

| Priority | Recommendation | Based On |
|----------|----------------|----------|
| High | Prioritize data-quality validation for clinically important variables before using the dataset for predictive analysis. | Data-quality findings |
| High | Use multiple patient characteristics together rather than relying on a single variable when investigating heart disease patterns. | Exploratory findings |
| Medium | Investigate the relationship between chest pain type, exercise-induced angina, and heart disease status in greater depth. | EDA findings |
| Medium | Explore additional datasets with more complete clinical information to strengthen future analysis. | Dataset limitations |

---

10. Assumptions & Limitations

Assumptions

- The dataset is assumed to represent the patient population described by its source.
- Heart disease status is treated as the outcome variable provided in the dataset.
- Categorical variables are interpreted according to their dataset definitions.

Limitations

- The analysis identifies associations and patterns, not causal relationships.
- The dataset contains missing values in some clinical variables.
- Some cholesterol values were recorded as zero, which may indicate missing or erroneous measurements.
- The dataset may not represent the wider population.
- The analysis is not intended to diagnose individual patients or predict individual medical outcomes.
- Some age groups contain fewer observations, which can affect comparisons.

---

11. Future Enhancements

- Perform deeper statistical testing of observed relationships.
- Investigate and validate questionable clinical values with the original data source.
- Expand the dataset with additional patient records.
- Build a machine-learning model for heart disease classification as a separate project.
- Compare model performance using different feature sets.

---

12. Dashboard

Power BI Dashboard

The interactive dashboard provides an overview of heart disease distribution and explores relationships between heart disease status and key demographic and clinical factors.

Dashboard Preview

"Heart Disease Dashboard" (visuals/heart_disease_dashboard.png)

Dashboard Features

- Heart disease KPI
- Heart disease distribution
- Gender analysis
- Age-group analysis
- Chest pain analysis
- Clinical factor analysis
- Interactive filters/slicers
- Key analytical insights

«Power BI Dashboard: [Add your shareable dashboard link here]»

---

13. Deliverables

| Deliverable | Description | Location |
|-------------|-------------|----------|
| Cleaned Dataset | Processed dataset used for analysis | `/data/processed/` |
| Jupyter Notebook | Data cleaning and exploratory analysis | `/notebooks/` |
| Dashboard | Interactive Power BI dashboard | Power BI link |
| Dashboard Screenshot | Portfolio-ready dashboard image | `/visuals/` |
| README | Project documentation | `/README.md` |

---

14. Author

Luciana

Data Analyst | Data Analytics & Business Intelligence

- 🔗 LinkedIn: linkedin.com/in/lucianaidogwu
- 💼 GitHub: https://github.com/luciana677
- 📧 Email: idogwuogechi@gmail.com

---

Last updated: August 2026
