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
<img width="665" height="494" alt="image" src="https://github.com/user-attachments/assets/cc510867-3c9f-43a0-9124-2182709af5c2" />


<h2> Model Accuracy </h2>
<img width="704" height="473" alt="image" src="https://github.com/user-attachments/assets/be2965c0-c924-4d15-a4cc-aba4a826b7a5" />


<h2> Deploying Model using Streamlit </h2>
<h2> steps for deployment </h2>

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

 load model
 
clf = model

 Set title

 add some display button 


 run in terminal 
 
envirment\Scripts\activate

when environment activate then write

Streamlit run file.py

when a model deployed then it opens a browser where it ask a test csv file.Then upload a test file . Then it predict fraud or non fraud.

<img width="940" height="636" alt="image" src="https://github.com/user-attachments/assets/3c748ecd-98b8-4051-8f9c-7e3fb9561dd8" />

as u can see there's Number of fraudulent transactions detected 27120 and rest are detected non-fraudulent out of 555719.



