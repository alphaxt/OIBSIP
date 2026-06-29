# 🧠 OIBSIP — Oasis Infobyte Data Science Internship

A collection of **4 end-to-end Data Science projects** completed as part of the [Oasis Infobyte](https://oasisinfobyte.com/) internship program. Each task covers a real-world problem — from classification and regression to NLP — with full EDA, model training, evaluation, and (for Task 4) a live **Streamlit web app**.

---

## 🗂️ Projects Overview

| # | Project | Type | Key Algorithm | Live App |
|---|---------|------|---------------|----------|
| 1 | [Iris Flower Classification](#task-1--iris-flower-classification) | Classification | Logistic Regression, KNN, SVM | — |
| 2 | [Unemployment Analysis](#task-2--unemployment-analysis-with-python) | EDA / Time Series | Pandas, Seaborn | — |
| 3 | [Car Price Prediction](#task-3--car-price-prediction) | Regression | Linear Regression, Random Forest | — |
| 4 | [Email Spam Detection](#task-4--email-spam-detection) | NLP / Classification | Naive Bayes + TF-IDF | ✅ Streamlit |

---

## 📁 Repository Structure

```
OIBSIP/
├── .devcontainer/
│   └── devcontainer.json            # GitHub Codespaces config (auto-runs Streamlit)
│
├── DataScience-Task1-IrisFlowerClassification/
│   ├── Muhammad_Danish_Iris_Flower_Classification.ipynb
│   ├── README.md
│   ├── output/                      # saved plots & results
│   └── screenshots/
│
├── DataScience-Task2-UnemploymentAnalysis/
│   ├── Unemployment_Analysis.ipynb
│   ├── Unemployment_Rate_upto_11_2020.csv
│   ├── README.md
│   ├── outputs/
│   └── screenshots/
│
├── DataScience-Task3-CarPricePrediction/
│   ├── notebook/                    # Jupyter notebook
│   ├── dataset/                     # car data.csv (CarDekho)
│   ├── outputs/                     # saved model & metrics
│   ├── images/                      # EDA screenshots
│   ├── requirements.txt
│   └── README.md
│
└── DataScience-Task4-EmailSpamDetection/
    ├── Email_Spam_Detection.ipynb
    ├── app/
    │   ├── app.py                   # Streamlit web app
    │   └── requirements.txt
    ├── dataset/
    │   └── spam.csv
    ├── outputs/                     # model metrics & reports
    └── README.md
```

---

## Task 1 — Iris Flower Classification

**Goal:** Classify Iris flowers into *Setosa*, *Versicolor*, and *Virginica* using petal/sepal measurements.

- Dataset loaded directly from `sklearn.datasets`
- EDA: pairplots, boxplots, descriptive statistics, null checks
- Models: Logistic Regression, K-Nearest Neighbors, Support Vector Machine
- Evaluation: Accuracy score, classification report, confusion matrix

📂 [`DataScience-Task1-IrisFlowerClassification/`](./DataScience-Task1-IrisFlowerClassification)

---

## Task 2 — Unemployment Analysis with Python

**Goal:** Analyze unemployment trends across Indian states and measure the COVID-19 impact.

- Dataset: Kaggle — *Unemployment in India (up to Nov 2020)*
- EDA: time series analysis, regional comparison, correlation heatmap
- Key finding: Sharp spike in unemployment during the COVID-19 lockdown period

📂 [`DataScience-Task2-UnemploymentAnalysis/`](./DataScience-Task2-UnemploymentAnalysis)

---

## Task 3 — Car Price Prediction

**Goal:** Predict the selling price of used cars using regression models.

- Dataset: CarDekho Vehicle Dataset (Kaggle)
- Features: Brand, Car Age, Present Price, KMs Driven, Fuel Type, Transmission, Owners
- Models: Linear Regression, Random Forest Regressor
- Metrics: MAE, RMSE, R² Score
- Best model saved with Joblib

📂 [`DataScience-Task3-CarPricePrediction/`](./DataScience-Task3-CarPricePrediction)

---

## Task 4 — Email Spam Detection

**Goal:** Classify SMS messages as *Spam* or *Ham* using NLP + Machine Learning, with a live Streamlit app.

- Dataset: SMS Spam Collection Dataset
- Pipeline: Text cleaning → Tokenization → Stopword removal → Stemming → TF-IDF → Naive Bayes
- Metrics: Accuracy, Precision, Recall, F1-Score, Confusion Matrix
- **Deployed via GitHub Codespaces** — opens automatically on port `8501`

📂 [`DataScience-Task4-EmailSpamDetection/`](./DataScience-Task4-EmailSpamDetection)

### Run the Streamlit App Locally

```bash
cd DataScience-Task4-EmailSpamDetection
pip install -r app/requirements.txt
streamlit run app/app.py
```

Then visit `http://localhost:8501` in your browser.

### Run in GitHub Codespaces

Click **"Open in Codespaces"** — the environment installs all dependencies and launches the Streamlit app automatically.

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/alphaxt/OIBSIP)

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| Language | Python 3.11 |
| Notebooks | Jupyter Notebook |
| Data | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| ML | Scikit-learn, Joblib |
| NLP | NLTK |
| Web App | Streamlit |
| Environment | GitHub Codespaces (.devcontainer) |

---

## 🚀 Getting Started (Local)

```bash
git clone https://github.com/alphaxt/OIBSIP.git
cd OIBSIP

# install deps for Task 3
pip install -r DataScience-Task3-CarPricePrediction/requirements.txt

# install deps for Task 4 + run app
pip install -r DataScience-Task4-EmailSpamDetection/app/requirements.txt
streamlit run DataScience-Task4-EmailSpamDetection/app/app.py
```

For Tasks 1 & 2, open the `.ipynb` files in Jupyter or VS Code — no extra requirements beyond standard data science libraries.

---

## 📜 License

This project is open-source under the **MIT License**.

---

**Developed by Muhammad Danish**
*Oasis Infobyte Data Science Internship*
