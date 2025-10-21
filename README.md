# Brain Stroke Prediction System 🧠⚕️

**A machine learning-based prediction system designed to identify the likelihood of brain stroke using health parameters like BMI, hypertension, glucose levels, and more.**

---

## Table of Contents

- [About](#about)  
- [Features](#features)  
- [Repository Structure](#repository-structure)  
- [Prerequisites](#prerequisites)  
- [Installation](#installation)  
- [Dataset](#dataset)  
- [Run / Usage](#run--usage)  
- [Model Overview (High Level)](#model-overview-high-level)  
- [Retrain / Rebuild](#retrain--rebuild)  
- [Troubleshooting](#troubleshooting)  
- [Contributing](#contributing)  
- [Acknowledgements](#acknowledgements)

---

## About

This project aims to **predict the risk of brain stroke** using machine learning techniques. It uses a dataset that includes a variety of medical and lifestyle factors to assess stroke probability with high accuracy.

The goal is to assist healthcare professionals and individuals in early detection, potentially saving lives through timely intervention.

> Built with robust ML algorithms and evaluated to achieve up to **96% accuracy** (based on experimentation).

---

## Features

- ✅ Predicts brain stroke risk based on health metrics  
- 📊 Data preprocessing, cleaning & feature engineering  
- 🤖 Trained using classification algorithms (e.g., RandomForest, XGBoost, etc.)  
- 📈 Performance evaluation with accuracy, confusion matrix, etc.  
- 🧪 Easily extendable for deployment (Flask / Streamlit)

---

## Repository Structure

```
Brain-Stroke-Prediction/
├─ .gitignore
├─ app.py                 # (If UI/Flask/Streamlit app is added)
├─ Brain_Stroke.ipynb     # Notebook with full model pipeline
├─ models/                # (Optional) Saved models
├─ requirements.txt
└─ data/
   └─ stroke.csv          # Raw dataset (Kaggle)
```

---

## Prerequisites

- Python 3.12.7+  
- pip / virtual environment  
- Jupyter Notebook (optional but recommended)

---

## Installation

```bash
# 1️⃣ Clone the repository
git clone https://github.com/debjit11/Brain-Stroke-Prediction.git
cd Brain-Stroke-Prediction

# 2️⃣ Create virtual environment (Recommended)
python -m venv .venv
# Windows
.\.venv\Scripts\activate
# Linux/Mac
source .venv/bin/activate

# 3️⃣ Install dependencies
pip install --upgrade pip
pip install -r requirements.txt
```

---

## Dataset

This project uses the **Brain Stroke Prediction Dataset** available on Kaggle.

The dataset includes features like:

| Feature          | Description                          |
|------------------|--------------------------------------|
| gender           | Male/Female                          |
| age              | Patient age                          |
| hypertension     | 0/1 indicates hypertension           |
| heart_disease    | 0/1 indicates heart condition        |
| ever_married     | Marital status                       |
| work_type        | Job type                             |
| Residence_type   | Urban/Rural                          |
| avg_glucose_level| Average blood glucose                |
| bmi              | Body Mass Index                      |
| smoking_status   | Current/former/never                 |
| stroke (Target)  | 0 = No Stroke, 1 = Stroke            |

---

## Run / Usage

### 1️⃣ Run Jupyter Notebook

```bash
jupyter notebook Brain_Stroke.ipynb
```

### 2️⃣ Run Web App (If app.py exists)

```bash
streamlit run app.py
```

---

## Model Overview (High Level)

- Data preprocessing (handling missing values, encoding categories)  
- Feature scaling and class balancing  
- Model training using ML algorithms  
- Performance comparison and final model selection  
- Evaluation with metrics:
  - Accuracy
  - Precision/Recall
  - Confusion Matrix

---

## Retrain / Rebuild

1. Download the dataset and place in `data/`  
2. Open the notebook and run all cells  
3. Save the final trained model  
4. Integrate with `app.py` if deploying

---

## Troubleshooting

| Issue | Solution |
|-------|----------|
| ModuleNotFoundError | Run `pip install -r requirements.txt` |
| Data path error | Ensure `stroke.csv` is in `/data/` folder |
| Low accuracy | Tune model hyperparameters |

---

## Contributing

1. Fork the repo  
2. Create branch: `git checkout -b feature/my-feature`  
3. Commit changes & create PR  

---

## Acknowledgements

- Kaggle Brain Stroke Dataset  
- Scikit-learn, Pandas, NumPy, Matplotlib  

---
