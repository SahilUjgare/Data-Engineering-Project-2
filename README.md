# 🏦 Loan Approval Prediction System

A data engineering and machine learning project that predicts loan approval decisions based on applicant financial and personal information — built with Python, Scikit-learn, and Flask/Streamlit.

---

## 📌 Overview

This project covers the complete data pipeline — from raw JSON ingestion and EDA to model training, serialization, and a deployed prediction app. It demonstrates real-world ETL practices, feature engineering, and ML model deployment.

---

## 📁 Project Structure

```
Data-Engineering-Project-2/
│
├── EDA_Train_pickle.py       # Exploratory data analysis + model training + pickle export
├── app.py                    # Web app for loan approval prediction
├── loan_approval_model.pkl   # Trained ML model (serialized)
│
├── applicant_info.json       # Applicant personal data
├── financial_info.json       # Applicant financial data
├── loan_info.json            # Loan request details
│
├── test_load_data.py         # Unit tests for data loading
├── requirements.txt          # Project dependencies
└── README.md
```

---

## ⚙️ How It Works

```
JSON Data Files  →  EDA & Cleaning  →  Feature Engineering  →  Model Training  →  Pickle Export  →  Web App
```

1. **Ingest** — Load applicant, financial, and loan data from JSON files
2. **EDA** — Explore distributions, handle missing values, encode categories
3. **Train** — Train a classification model (Scikit-learn) to predict approval
4. **Serialize** — Export trained model as `loan_approval_model.pkl`
5. **Serve** — Load model in `app.py` and predict on new applicant data

---

## 🛠️ Tech Stack

| Layer | Tools |
|---|---|
| Language | Python |
| Data handling | Pandas, NumPy |
| ML Model | Scikit-learn |
| Serialization | Pickle |
| App | Flask / Streamlit |
| Testing | Pytest |
| Data format | JSON |

---

## 🚀 Getting Started

**1. Clone the repo**
```bash
git clone https://github.com/SahilUjgare/Data-Engineering-Project-2.git
cd Data-Engineering-Project-2
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Train the model**
```bash
python EDA_Train_pickle.py
```

**4. Run the app**
```bash
python app.py
```

**5. Run tests**
```bash
python test_load_data.py
```

---

## 📊 Model Details

- **Task** — Binary classification (Loan Approved / Rejected)
- **Input features** — Applicant info, financial history, loan amount, tenure
- **Output** — Approval prediction with confidence score
- **Model file** — `loan_approval_model.pkl`

---

## 📂 Data Files

| File | Description |
|---|---|
| `applicant_info.json` | Name, age, employment, credit history |
| `financial_info.json` | Income, expenses, existing loans |
| `loan_info.json` | Requested amount, tenure, purpose |

---


## 📄 License

This project is open source and available under the [MIT License](LICENSE).
