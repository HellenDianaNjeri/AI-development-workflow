# AI-development-workflow
# Patient Readmission Risk Prediction

## Project Overview

This project focuses on developing a machine learning model to predict whether diabetic patients are likely to be readmitted to the hospital. Using historical data from over 100,000 hospital visits, the model aims to assist healthcare providers in reducing avoidable readmissions and improving patient outcomes.

---

## Dataset

- **Source**: Diabetes Readmission Dataset from Kaggle  
- **Size**: 101,766 patient records, 50 features  
- **Target Variable**: `readmitted` (`NO`, `<30`, `>30`)  
- **Features**: Patient demographics, diagnoses, admission types, lab procedures, medications, and time in hospital

---

## Workflow Summary

### 1. Data Exploration & Cleaning

- Identified missing values and replaced `?` placeholders
- Dropped columns with excessive missing or irrelevant data
- Addressed duplicate entries and filtered edge cases

### 2. Preprocessing

- Encoded categorical variables using Label and One-Hot Encoding
- Normalized numerical data using MinMaxScaler
- Split the dataset into training and test sets

### 3. Modeling

- Selected Random Forest Classifier for its performance and interpretability
- Evaluated with metrics: Accuracy, Precision, Recall, F1-score
- Performed hyperparameter tuning and cross-validation

### 4. Deployment Planning

- Outlined integration plan for hospital EHR systems
- Addressed privacy and regulatory compliance

---

## Key Findings

- High readmission rates occurred within 30 days of discharge
- Certain features like time in hospital, medication changes, and diagnoses were strong predictors
- The Random Forest model performed best in balancing precision and recall

---

## Next Steps

- Deploy the model via an API or dashboard for healthcare staff
- Monitor real-time performance and update with new data
- Consider ensemble or deep learning models to improve accuracy

---

## Tech Stack

- **Language**: Python  
- **Libraries**: pandas, numpy, scikit-learn, matplotlib, seaborn  
- **Development Tools**: Jupyter Notebook, VS Code

---

## Project Structure

AI-DEVELOPMENT-WORKFLOW/
│
├── DIABETES_DATA.CSV # Original dataset used for modeling
├── PATIENT_READMISSION.ipynb # Main Jupyter notebook containing all code, EDA, preprocessing, modeling, and evaluation
├── AI DEVELOPMENT WORKFLOW.pdf # Final project report including reflection and findings
├── AI DEVELOPMENT WORKFLOW.png # Visual flowchart of the AI workflow process
├── README.md # Project overview, instructions, and documentation
---

## Ethical and Privacy Considerations

- Dataset is anonymized and publicly available
- Future deployment will follow data protection regulations such as HIPAA

---

## Author

Hellen Diana Njeri Macharia  

