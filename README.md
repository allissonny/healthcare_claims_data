# Predicting Healthcare Claim Outcomes
### Machine Learning Analysis of Synthetic Healthcare Claims Data

This project analyzes a synthetic healthcare claims dataset to explore patterns in reimbursement outcomes and evaluate whether machine learning models can predict whether a claim will be **paid, denied, or partially reimbursed**.

The project demonstrates a full data science workflow including:

- Data preparation
- Exploratory data analysis
- Feature engineering
- Machine learning modeling
- Model interpretation
- Communication of findings

---

## Project Objective

Healthcare organizations process large volumes of insurance claims, and claim denials or partial reimbursements can create significant administrative workload and financial delays.

The objective of this project was to:

• Explore relationships between claim characteristics and claim outcomes  
• Identify patterns associated with reimbursement outcomes  
• Evaluate whether machine learning models can predict claim outcomes  

---

## Dataset

Synthetic Healthcare Claims Dataset  
Source: Kaggle  
https://www.kaggle.com/datasets/abuthahir1998/synthetic-healthcare-claims-dataset

The dataset contains **1,000 simulated healthcare claims** with variables describing billing amounts, insurance coverage, procedure codes, diagnosis codes, and claim outcomes.

Key variables include:

- Billed Amount
- Allowed Amount
- Paid Amount
- Insurance Type
- Procedure Code
- Diagnosis Code
- Claim Status
- Outcome (Paid, Denied, Partially Paid)

The dataset is **synthetic and randomly generated**, meaning it does not contain real patient data and is intended for educational and machine learning training purposes.

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook

---

## Project Workflow

### 1. Data Exploration

Initial analysis examined the distribution of claim outcomes and explored relationships between billing variables, insurance types, and reimbursement patterns.

### 2. Data Preparation

Data preprocessing included:

- Cleaning column names
- Converting date fields
- Feature engineering (payment ratios)
- Handling categorical variables

### 3. Exploratory Data Analysis

Visualizations explored:

- Claim outcome distribution
- Claim outcomes by insurance type
- Billed vs paid amount comparison
- Payment ratios by insurer
- Follow-up requirements by claim outcome

### 4. Machine Learning Models

Two classification models were evaluated:

- Logistic Regression
- Random Forest

These models attempted to predict claim outcomes based on claim characteristics.

---

## Model Results

| Model | Accuracy | Weighted F1 |
|------|------|------|
| Logistic Regression | 0.355 | 0.354 |
| Random Forest | 0.330 | 0.328 |

Logistic regression slightly outperformed the random forest model.

Predictive performance remained limited, which is expected because the dataset is **synthetic and randomly generated**.

---

## Feature Importance Insights

Feature importance analysis indicated that the following variables had the strongest influence on predictions:

- Billed Amount
- Procedure Code
- Insurance Type
- Service Day of Week

These variables may represent billing characteristics associated with reimbursement outcomes.

---

## Key Findings

Key observations from the exploratory analysis:

• Claim outcomes were relatively balanced across the dataset  
• Insurance type showed differences in denial rates  
• Self‑pay claims had the highest denial percentage  
• Financial variables alone did not strongly predict outcomes  

Because the dataset is synthetic, the predictive models did not achieve high accuracy; however, the workflow demonstrates how machine learning could be applied to healthcare claims data.

---

## Limitations

This project has several limitations:

- Synthetic dataset
- Limited sample size
- Simplified healthcare reimbursement logic

Real healthcare claims datasets would likely produce stronger predictive relationships.

---

## Future Work

Future improvements could include:

- Using real healthcare claims datasets
- Incorporating additional variables (patient demographics, provider specialty)
- Testing additional machine learning algorithms
- Building interactive dashboards for revenue cycle monitoring

---

## Ethical Considerations

Although the dataset used in this project is synthetic, predictive analytics in healthcare finance must be implemented carefully.

Predictive models should support decision‑making rather than replace human review, and organizations must ensure transparency, fairness, and oversight when deploying analytics.

---

This project was completed as part of a graduate‑level data science program and demonstrates applying analytics and machine learning techniques to healthcare operational data.
