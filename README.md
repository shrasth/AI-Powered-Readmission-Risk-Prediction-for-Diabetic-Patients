# AI-Powered Readmission Risk Prediction for Diabetic Patients  
*(with Snowflake, Machine Learning, Explainable AI & Generative AI)*

## 🩺 Project Summary

This project builds a complete AI-powered pipeline to predict 30-day hospital readmission risk for diabetic patients. The solution integrates modern data science tools, cloud data engineering, explainable AI, and generative AI automation to simulate a real-world healthcare analytics application.

---

## Key Features

- **Snowflake** for cloud-based data storage, ingestion, and transformation.
- **Python** for data analysis, machine learning, and pipeline automation.
- **Machine Learning** models: Random Forest, XGBoost, Logistic Regression.
- **Explainable AI (XAI)** using SHAP to interpret model decisions.
- **Generative AI (LLM)** integration via OpenAI's GPT-4o to generate patient risk reports.
- **Automation** using Prefect for end-to-end orchestration.
- **Deployment** with an interactive Streamlit app.

---

## Dataset

- **Source:** UCI Machine Learning Repository  
- **Dataset:** [Diabetes 130-US hospitals for years 1999–2008](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008)  
- Contains ~100K patient records with demographics, diagnoses, and readmission labels.

---

## Project Workflow

1. **Data Ingestion**  
   - Load raw dataset into Snowflake cloud data warehouse.

2. **Data Transformation**  
   - Clean and prepare data using Snowflake SQL and Python.

3. **Machine Learning**  
   - Train models to predict readmission risk.
   - Evaluate model performance using ROC-AUC, F1, and precision-recall metrics.

4. **Explainability**  
   - Use SHAP to analyze feature importance for transparency in healthcare predictions.

5. **Generative AI Reports**  
   - Generate natural language patient summaries using OpenAI GPT models.

6. **Automation Pipeline**  
   - Build end-to-end orchestration with Prefect.

7. **Deployment**  
   - Deploy an interactive web app using Streamlit for real-time risk prediction and explanation.

---

## Tools & Technologies Used

| Category | Tools |
| -------- | ----- |
| Data Storage | Snowflake |
| Programming | Python 3.10+ |
| ML Libraries | scikit-learn, XGBoost |
| XAI | SHAP |
| LLM Integration | OpenAI GPT-4o, LangChain |
| Automation | Prefect |
| Deployment | Streamlit |
| Version Control | Git + GitHub |

---

## Repository Structure

```bash
├── data/                # Raw & processed datasets
├── notebooks/           # Jupyter notebooks for EDA and model development
├── src/                 # Source code for ML pipelines
├── automation/          # Prefect flow scripts
├── deployment/          # Streamlit app code
├── docs/                # Diagrams and documentation
├── requirements.txt     # Python package dependencies
├── README.md            # Project readme (this file)
