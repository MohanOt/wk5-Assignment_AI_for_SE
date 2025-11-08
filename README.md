# 🧠 AI Development Workflow – Predicting Student Dropout & Patient Readmission Risk

This repository contains the complete submission for the **AI Development Workflow Assignment**, demonstrating understanding and application of the full AI project lifecycle — from **problem definition to deployment and monitoring**.

The project covers two practical cases:
1. A **hypothetical education problem** – predicting student dropout rates.
2. A **real-world healthcare case study** – predicting patient readmission risk within 30 days of discharge.

---

## 📂 Repository Structure

ai_project/
├── docs/
│ └── AI_Development_Workflow_Assignment_with_Diagram.pdf
├── notebooks/
│ └── model_dev.ipynb

markdown
Copy code

- **docs/** → Contains the final written report (PDF) with detailed explanations, reflections, and the workflow diagram.  
- **notebooks/** → Contains a simple Python notebook illustrating model evaluation (confusion matrix, precision, recall).

---

## 🧩 Project Overview

### 🎯 Problem Definition
The AI system aims to **predict outcomes** such as:
- Which students are at risk of dropping out.
- Which patients are at risk of readmission within 30 days.

**Objectives:**
- Improve early interventions and retention.
- Optimize institutional and hospital resources.
- Enhance decision-making through predictive analytics.

**Stakeholders:**  
University administrators, academic advisors, doctors, hospital management, and patients.

---

## 🧮 Data Collection & Preprocessing

**Data Sources:**
- Educational: Student Information Systems (SIS), Learning Management Systems (LMS).  
- Healthcare: Electronic Health Records (EHRs), demographic and discharge data.

**Key Steps:**
1. Handle missing values and inconsistencies.  
2. Encode categorical variables (e.g., diagnosis, gender).  
3. Normalize numerical values for stable model performance.  

**Potential Bias:**  
Unequal data representation may skew predictions — mitigated through balanced sampling and fairness checks.

---

## 🤖 Model Development

**Chosen Models:**
- **Education:** Random Forest – balances performance and interpretability.  
- **Healthcare:** Logistic Regression – transparent, lightweight, and interpretable for clinical use.  

**Data Split:**  
70% Training | 15% Validation | 15% Testing

**Hyperparameters Tuned:**  
- Number of trees (Random Forest)  
- Regularization strength (Logistic Regression)

**Performance Metrics:**  
- **Accuracy** → Measures overall correctness.  
- **F1-Score / Precision / Recall** → Capture model balance and reliability.

**Example Output:**
Confusion Matrix: [[70, 30], [20, 80]]
Precision: 0.78
Recall: 0.70

yaml
Copy code

---

## 🚀 Deployment Strategy

The model can be deployed via a **REST API** integrated into:
- University data dashboards (for student retention systems).
- Hospital EHR systems (for real-time readmission alerts).

**Challenges:** Scalability, real-time prediction load, and maintaining performance post-deployment.

**Monitoring Concept Drift:**  
Continuous retraining and KPI tracking to ensure predictions remain accurate over time.

**Regulatory Compliance:**  
HIPAA-compliant data handling, encryption, anonymization, and secure storage.

---

## ⚖️ Ethics & Bias

**Risks:**
- Biased training data may reinforce inequalities in healthcare or education outcomes.

**Mitigation:**
- Fairness audits, explainable AI tools, and diverse data collection practices.

---

## 🔍 Trade-offs

| Aspect | High Accuracy Model | Interpretable Model |
|--------|----------------------|--------------------|
| Transparency | ❌ Low | ✅ High |
| Resource Demand | ⚡ High | 🪶 Low |
| Use Case | Automated predictions | Healthcare decision support |

Due to computational and ethical considerations, interpretable models like **Logistic Regression** are favored.

---

## 🪞 Reflection

> *"The most challenging part was ensuring data quality and defining measurable objectives.  
> With more time, I would expand the data pipeline, explore deep learning models, and automate model monitoring."*

---

## 🧭 Workflow Diagram

The AI development workflow followed the **CRISP-DM framework**:

1. Problem Definition  
2. Data Collection  
3. Data Preprocessing  
4. Model Development  
5. Model Evaluation  
6. Deployment  
7. Monitoring & Maintenance  

![Workflow Diagram](docs/../workflow_diagram.png)

---

## 🧾 Deliverables

| File | Description |
|------|--------------|
| **AI_Development_Workflow_Assignment_with_Diagram.pdf** | Full report with analysis and diagram |
| **model_dev.ipynb** | Notebook demonstrating evaluation metrics |

---

## 👥 Contributors

- **Otieno Mohan** – Data Analyst / AI Developer  
- *Peer group collaboration as per PLP Academy requirements.*

---

## 📚 References

- CRISP-DM Model – Cross Industry Standard Process for Data Mining  
- Scikit-learn Documentation: [https://scikit-learn.org](https://scikit-learn.org)  
- TensorFlow Documentation: [https://www.tensorflow.org](https://www.tensorflow.org)

---