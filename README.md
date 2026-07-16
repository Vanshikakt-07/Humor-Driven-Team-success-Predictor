# Team Success Prediction using Machine Learning

A machine learning project that analyzes team collaboration metrics to predict the likelihood of project success.

---

## Overview

This project investigates how team dynamics influence overall project success. Using survey data collected from team members, the project applies machine learning techniques to determine whether factors such as contribution levels and team communication (represented through humor frequency) can predict successful teams.

The complete pipeline includes data preprocessing, feature engineering, model training, evaluation, and feature importance analysis.

---

## Features

- Data cleaning and preprocessing
- Feature engineering from team survey responses
- Humor frequency encoding
- Team contribution analysis
- Binary team success prediction
- Logistic Regression implementation
- Random Forest classification
- Model evaluation using standard ML metrics
- Feature importance analysis

---

## Dataset

The dataset consists of anonymous survey responses containing:

- Team member contribution ratings
- Self contribution rating
- Humor/communication frequency
- Overall team success score (1–10)

### Engineered Features

- Average Team Contribution
- Humor Score
- Success Label (Binary)

Teams with a success score of **9 or above** are classified as successful.

---

## Machine Learning Pipeline

```
Raw Survey Data
       │
       ▼
Data Cleaning
       │
       ▼
Feature Engineering
       │
       ▼
Train-Test Split
       │
       ▼
Model Training
 ├── Logistic Regression
 └── Random Forest
       │
       ▼
Model Evaluation
```

---

## Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- NetworkX

---

## Models Used

### Logistic Regression
- StandardScaler Pipeline
- Balanced Class Weights
- Binary Classification

### Random Forest
- 200 Decision Trees
- Balanced Subsample
- Feature Importance Analysis

---

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

---

## Project Structure

```
.
├── team_responses.xlsx
├── Team_Success_Prediction.ipynb
├── README.md
└── requirements.txt
```

---

## Key Insights

- Average team contribution is the strongest predictor of team success.
- Communication patterns contribute additional predictive information.
- Random Forest provides feature importance, highlighting the impact of contribution scores.
- Behavioral data can be effectively used for team performance analytics.

---

## Future Improvements

- Collect a larger dataset
- Add Graph Neural Networks for team interaction modeling
- Experiment with XGBoost and LightGBM
- Deploy as a Streamlit dashboard
- Extend to multiclass team success prediction

---

## Installation

```bash
git clone https://github.com/<your-username>/team-success-prediction.git

cd team-success-prediction

pip install -r requirements.txt
```

---

## Run

```bash
jupyter notebook Team_Success_Prediction.ipynb
```

---

## License

This project is intended for educational and research purposes.
