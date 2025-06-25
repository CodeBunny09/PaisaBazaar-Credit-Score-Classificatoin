# 🧠 Credit Score Classification for Paisabazaar

## 🎯 Objective
Build a machine learning pipeline to classify customer credit scores into:
- **0: Poor**
- **1: Standard**
- **2: Good**

This helps **Paisabazaar** improve their credit risk assessment process and automate customer segmentation based on financial behavior.

---

## 📁 Project Structure

```

Credit Score Classification for Paisabazaar/
│
├── data/
│   ├── raw/                     # Original dataset
│   │   └── dataset-2.csv
│   ├── processed/               # Cleaned data used for modeling
│   │   └── cleaned\_dataset.csv
│   └── README.md
│
├── models/
│   ├── best\_model.pkl           # Final trained model
│   └── logs/                    # (Optional) model logs or checkpoints
│
├── reports/
│   ├── figures/                 # EDA and model analysis plots
│   └── final\_summary.md         # Final project summary
│
├── credit\_score\_analysis.ipynb  # 📓 Main Jupyter notebook
├── requirements.txt             # 📦 Project dependencies
└── README.md                    # 🗂️ You're here

````

---

## 🧪 Dataset Info
- **Size:** 100,000 rows
- **Source:** Provided CSV
- **Features:** Demographics, credit behavior, loans, balances, etc.
- **Target:** `Credit_Score` (Multiclass)

---

## 🔄 Workflow

### 1. Data Cleaning
- Removed NaNs, duplicates, and non-informative columns
- Imputed missing values
- Categorical encoding + feature scaling

### 2. Exploratory Data Analysis (EDA)
- Distribution plots
- Correlations
- Feature importance analysis

### 3. Modeling
- Logistic Regression
- Random Forest
- XGBoost (📈 Best performer)

### 4. Optimization
- Hyperparameter tuning with `RandomizedSearchCV`
- ROC-AUC Evaluation
- SMOTE & Class Weighting to handle class imbalance

---

## 📊 Model Performance

| Model              | Accuracy | Macro F1 | Notes                      |
|-------------------|----------|----------|----------------------------|
| Logistic Regression | 0.66     | 0.63     | Baseline model             |
| Random Forest      | 0.83     | 0.83     | Strong performance         |
| **XGBoost (Tuned)**| **0.81** | **0.80** | ✅ Best generalization     |
| XGBoost + SMOTE    | 0.80     | 0.79     | Balanced but lower recall  |
| XGBoost + Class Weights | **0.81** | **0.80** | 🏆 Final model             |

---

## 📦 Installation

```bash
git clone https://github.com/your-username/credit-score-prediction
cd credit-score-prediction
pip install -r requirements.txt
````

---

## 🔮 Future Scope

* Ensemble models (stacking)
* Real-time dashboard with Streamlit or Flask
* Model interpretability with SHAP
* Deployment with Docker or FastAPI

---

## 🤝 Acknowledgements

Thanks to **Paisabazaar** and the open-source ML community ❤️

---

## 📬 Contact

**Pratik Choudhuri**
[LinkedIn](https://www.linkedin.com/in/pratik-c/) • [GitHub](https://github.com/CodeBunny09)


