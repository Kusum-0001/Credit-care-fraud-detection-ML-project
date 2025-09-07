<h2> Credit-care-fraud-detection-ML-project </h2>
<h2>🔍 Overview </h2>
<p1>Built a machine learning model to detect fraudulent credit card transactions. Applied multiple classification algorithms and feature engineering for performance improvement. </p1>

<h2>🛠️ Tech Stack</h2>
Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)

Jupyter Notebook

Features: Transaction details, Amount, Class (Fraud/Not Fraud).

<h2>📊 Key Insights </h2>

Logistic Regression, Random Forest & Decision Tree tested.

Achieved 99% accuracy.

Class imbalance handled with SMOTE / undersampling.

<h2> Confusion Matrix </h2>
[confusion matrix](https://github.com/Kusum-0001/Credit-care-fraud-detection-ML-project/blob/main/Confusion%20Metrix.png)

<h2> Model Accuracy </h2>
(https://github.com/Kusum-0001/Credit-care-fraud-detection-ML-project/blob/main/model%20accuracy.png)

<h2> Deploying Model using Streamlit </h2>

<h2> Import some libraries </h2>
import streamlit as st

import pandas as pd

import joblib

from sklearn.metrics import classification_report, confusion_matrix

<h2>load trained model </h2>
@st.cache_resource

def load_model():

    model = joblib.load('fraud_detection_model.pkl')
    
    return model

<h2> load model </h2>
clf = model

<h2> Set title </h2>

<h2> add some display button </h2>


<h2> run in terminal <h2>
envirment\Scripts\activate

when environment activate then write

Streamlit run file.py

