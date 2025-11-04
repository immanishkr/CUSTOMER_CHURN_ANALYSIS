📊 Telco Customer Churn Prediction
📘 Project Overview

This project focuses on predicting customer churn in a telecom company using machine learning techniques. Churn prediction helps the business identify customers likely to discontinue their service and take proactive retention measures.

The system includes:

Data exploration and cleaning (EDA)

Model building and evaluation

Deployment through a Flask web application

🧩 Key Objectives

Understand customer behavior patterns through Exploratory Data Analysis (EDA)

Build a predictive model using machine learning algorithms to forecast churn

Develop a web-based interface that allows users to input customer details and get churn predictions in real time

🛠️ Tech Stack

Languages & Frameworks:

Python

Flask

HTML, CSS (for frontend)

Libraries:

Pandas, NumPy

Scikit-learn

Matplotlib, Seaborn

Pickle (for model serialization)

Dataset:

WA_Fn-UseC_-Telco-Customer-Churn.csv (Telco Customer Churn dataset from IBM)

🔍 Exploratory Data Analysis (EDA)

Performed in Churn Analysis - EDA.ipynb

Key Steps:

Data sourcing and cleaning (handled missing, invalid, and outlier values)

Feature scaling and encoding for categorical variables

Univariate and bivariate analysis to identify patterns influencing churn

Derived new features like tenure groupings to improve prediction accuracy

Visualization Techniques:

Histograms, Bar charts, Box plots, Pair plots, Heatmaps

Correlation analysis to detect feature relationships

🧠 Model Building

Implemented in Churn Analysis - Model Building.ipynb

Models Evaluated:

Logistic Regression

Random Forest Classifier (selected model)

Gradient Boosting

Final Model:

Random Forest Classifier achieved the best accuracy and interpretability.

The trained model was serialized and saved as model.sav for deployment.

🌐 Model Deployment (Flask App)

Implemented in app.py

Features:

User-friendly web interface to input customer attributes

Backend integration with the trained ML model

Real-time churn prediction with probability scores

Run the App:
python app.py


Then open the app in your browser:
http://127.0.0.1:5000/

Prediction Output:

“This customer is likely to be churned!!”

“This customer is likely to continue!!”
with corresponding confidence percentages.

📂 Project Structure
├── app.py                          # Flask web application
├── Churn Analysis - EDA.ipynb      # EDA and data cleaning
├── Churn Analysis - Model Building.ipynb  # Model training and evaluation
├── first_telc.csv                  # Processed dataset
├── model.sav                       # Saved trained model
├── templates/
│   └── home.html                   # Frontend UI
├── Exploratory Data Analysis - Satyajit.pdf  # EDA report
└── README.md                       # Project documentation

📈 Results and Insights

Identified key factors influencing churn: contract type, tenure, payment method, and monthly charges.

The Random Forest model achieved high accuracy (>80%) in predicting customer churn.

Deployment enables quick decision-making for telecom retention strategies.

🚀 Future Enhancements

Integrate with real-time customer databases (SQL/NoSQL)

Implement automated retraining pipelines for dynamic data

Extend the system into a dashboard using Streamlit or Power BI for visualization

👨‍💻 Author

Manish Kumar
Machine Learning & Software Developer | Computer Science Educator
