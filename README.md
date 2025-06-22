# AI-Powered Hospital Readmission Risk Prediction

## Project Overview

Hospital readmissions contribute significantly to healthcare costs and patient burden, especially among chronic diseases like diabetes. This project develops an end-to-end AI-powered solution to predict 30-day readmission risk for diabetic patients using real-world healthcare data. The solution integrates cloud data warehousing, machine learning, explainability, generative AI reporting, and automation — simulating a full-stack data science application relevant for real-world healthcare operations.

This project is designed as a production-grade portfolio case study, demonstrating capabilities across **data engineering, machine learning, AI integration, and cloud automation**.

---

## Business Problem

> Can we proactively identify diabetic patients at risk of being readmitted within 30 days of discharge? Early identification of high-risk patients allows healthcare providers to allocate resources, intervene earlier, and potentially improve patient outcomes.

---

## Solution Highlights

- **Cloud Data Engineering**: Data ingestion, cleansing, and transformation using Snowflake.
- **Machine Learning**: Predictive models trained using Random Forest, XGBoost, and Logistic Regression.
- **Explainable AI**: SHAP-based feature attribution to generate clinically interpretable explanations.
- **Generative AI**: GPT-powered narrative summaries translating predictions into natural language risk assessments for clinicians.
- **Automation Pipelines**: Full end-to-end data orchestration with Prefect.
- **Deployment**: Interactive web application using Streamlit for real-time prediction, explainability, and report generation.

---

## Dataset Description

- **Source**: UCI Machine Learning Repository
- **Dataset**: [Diabetes 130-US hospitals for years 1999–2008](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008)
- **Records**: ~100,000 patient admissions
- **Fields**: Demographics, diagnoses, lab results, medications, and readmission outcomes

> *Note: This is a public dataset; no protected health information (PHI) is involved.*

---

## Technology Stack

| Layer | Tools |
| ----- | ----- |
| Data Warehouse | **Snowflake** |
| Data Science | **Python, pandas, scikit-learn, XGBoost** |
| Explainability | **SHAP (SHapley values)** |
| AI/LLM Integration | **OpenAI GPT-4o, LangChain** |
| Automation & Orchestration | **Prefect** |
| Deployment | **Streamlit** |
| Version Control | **GitHub** |

---

## Machine Learning Approach

- **Preprocessing**: Missing value handling, feature encoding, outlier removal
- **Feature Engineering**: Derived features using Snowflake SQL & Python
- **Models Evaluated**:
  - Random Forest Classifier
  - XGBoost Classifier
  - Logistic Regression (baseline)
- **Evaluation Metrics**:
  - ROC-AUC
  - F1-Score
  - Precision-Recall Curve

---

## Explainable AI

> In healthcare, model transparency is critical. SHAP (SHapley Additive Explanations) is used to quantify each feature’s contribution to an individual patient’s readmission risk, enhancing model trust and clinical interpretability.

---

## Generative AI Integration

- **Objective**: Translate model predictions into doctor-friendly risk assessment summaries.
- **Tool**: OpenAI GPT-4o API with LangChain orchestration
- **Example Output**:

> "Based on the patient's medical history, recent lab results, and medication adjustments, the predicted likelihood of readmission within 30 days is 72%. Key contributing factors include prior emergency visits, insulin regimen changes, and elevated A1C levels."

---

## Automation Pipeline

| Stage | Automated Process |
| ----- | ------------------ |
| Data Ingestion | Snowflake Tasks |
| Feature Engineering | Snowflake SQL Views |
| Model Training | Python ML Pipeline |
| Explainability | SHAP Visualizations |
| Report Generation | GPT-powered narrative |
| Orchestration | Prefect Workflows |
| Deployment | Streamlit Web App |

---

## Deployment Demo

> 🚀 *A fully functional Streamlit application is deployed [here](#) to demonstrate real-time predictions, explainability, and AI-generated reports.*

---

## Repository Structure

```bash
   diabetes-readmission-prediction
 ┣ 📂 data/                # Raw and processed data
 ┣ 📂 notebooks/           # Exploratory data analysis and model notebooks
 ┣ 📂 src/                 # Source code for ML pipelines
 ┣ 📂 automation/          # Prefect flows and orchestration scripts
 ┣ 📂 deployment/          # Streamlit app code
 ┣ 📂 docs/                # Documentation and architecture diagrams
 ┣ 📄 requirements.txt     # Python dependencies
 ┣ 📄 README.md            # Project overview (this file)
