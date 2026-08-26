🔐 AI Financial Fraud Detection using Machine Learning

<p align="center">🚨 Detecting Potentially Fraudulent Financial Transactions with AI & Predictive Analytics

<img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python" />
<img src="https://img.shields.io/badge/Machine%20Learning-Scikit--learn-orange?style=for-the-badge&logo=scikit-learn" />
<img src="https://img.shields.io/badge/Data%20Analysis-Pandas-green?style=for-the-badge&logo=pandas" />
<img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" /></p>---

📌 Project Overview

AI Financial Fraud Detection is an end-to-end Machine Learning project developed to identify potentially fraudulent financial transactions.

The project analyzes a 200,000-record financial transaction dataset containing 24 features and follows a complete Machine Learning workflow including data understanding, data cleaning, exploratory data analysis, preprocessing, feature engineering, model training, model evaluation, fraud prediction, threshold analysis, and model saving.

The primary objective is to demonstrate how Artificial Intelligence, Machine Learning, and Predictive Analytics can be applied to a financial fraud detection problem.

---

🎯 Business Problem

Financial fraud is a major challenge for banks and financial institutions. A transaction monitoring system needs to identify suspicious transactions while minimizing incorrect classifications.

Project Objectives

- 🔍 Understand financial transaction data
- 🧹 Clean and preprocess the dataset
- 📊 Perform Exploratory Data Analysis
- 🚨 Analyze fraudulent transaction patterns
- ⚖️ Handle and understand class imbalance
- 🤖 Train multiple Machine Learning classification models
- 📈 Compare model performance
- 🎯 Analyze classification thresholds
- 🧪 Test predictions on unseen transaction data
- 💾 Save the trained Machine Learning model

---

🔄 Project Workflow

Financial Transaction Dataset
            ↓
      Data Understanding
            ↓
        Data Cleaning
            ↓
 Exploratory Data Analysis
            ↓
 Class Imbalance Analysis
            ↓
     Feature Engineering
            ↓
   Data Preprocessing
            ↓
      Train-Test Split
            ↓
      Model Training
            ↓
     Model Comparison
            ↓
    Model Evaluation
            ↓
 Threshold Analysis
            ↓
   Best Model Selection
            ↓
 Unseen Transaction Prediction
            ↓
       Model Saving

---

📊 Dataset

The project uses a financial transaction dataset containing:

- 200,000 records
- 24 features
- Customer-related information
- Account-related information
- Transaction information
- Merchant information
- Device information
- Location information
- Fraud classification

🎯 Target Variable

"Is_Fraud"

Value| Meaning
"0"| Legitimate Transaction
"1"| Fraudulent Transaction

The dataset represents an imbalanced binary classification problem, which makes fraud-sensitive metrics such as Precision, Recall, F1-Score, ROC-AUC and PR-AUC important for evaluating model performance.

---

🔎 Dataset Features

The dataset contains customer, account, transaction, merchant, device and location-related attributes, including:

- Customer ID
- Customer Name
- Gender
- Age
- State
- City
- Bank Branch
- Account Type
- Transaction ID
- Transaction Date
- Merchant Category
- Account Balance
- Transaction Device
- Transaction Location
- Device Type
- Transaction Currency
- Customer Contact
- Transaction Description
- Customer Email
- Fraud Indicator

---

🧹 Data Preprocessing

The project applies multiple preprocessing techniques before training the Machine Learning models.

Main Steps

- Data inspection
- Data type analysis
- Missing-value analysis
- Duplicate analysis
- Feature selection
- Numerical feature preprocessing
- Categorical feature encoding
- Feature scaling
- Train-test splitting
- Feature transformation using Scikit-learn pipelines

The project uses tools such as:

- "StandardScaler"
- "OneHotEncoder"
- "ColumnTransformer"
- "Pipeline"

---

📈 Exploratory Data Analysis

Exploratory Data Analysis is performed to understand transaction behavior and identify patterns related to fraud.

Analysis Includes

- Fraud vs. legitimate transaction distribution
- Customer demographics
- Transaction behavior
- Merchant categories
- Account types
- Transaction locations
- Device types
- Numerical feature relationships
- Correlation analysis
- Class imbalance visualization

Data visualization is used to make transaction patterns and relationships easier to interpret.

---

🤖 Machine Learning Models

Three classification algorithms are trained and evaluated.

1️⃣ Logistic Regression

Used as a baseline classification model to establish an initial performance benchmark.

2️⃣ Decision Tree Classifier

A tree-based classification algorithm capable of learning non-linear relationships between transaction features.

3️⃣ Random Forest Classifier

An ensemble learning algorithm that combines multiple decision trees and is used as the primary model for comparison and fraud prediction.

---

📊 Model Evaluation

Fraud detection is an imbalanced classification problem, so Accuracy alone cannot provide a complete picture of model performance.

The project evaluates models using:

Accuracy

Measures the overall percentage of correctly classified transactions.

Precision

Measures how many transactions predicted as fraudulent were actually fraudulent.

Recall

Measures how many actual fraudulent transactions were successfully identified.

F1-Score

Provides a balance between Precision and Recall.

ROC-AUC

Measures the ability of the model to distinguish between fraudulent and legitimate transactions across different classification thresholds.

PR-AUC

Provides an additional evaluation perspective for imbalanced classification problems by focusing on the Precision-Recall relationship.

Confusion Matrix

Analyzes:

- True Positives
- True Negatives
- False Positives
- False Negatives

---

⚠️ Important Model Performance Insight

The final Random Forest model achieved approximately:

Metric| Result
Accuracy| 94.79%
Precision| 5.33%
Recall| 0.20%
F1-Score| 0.38%

What does this mean?

Although the overall Accuracy is high, the very low Recall indicates that the model is not yet effective enough at identifying actual fraudulent transactions.

This is an important finding because fraud detection is highly sensitive to False Negatives.

A model can achieve high Accuracy on an imbalanced dataset while still missing a large proportion of fraudulent transactions.

Therefore, this project does not treat Accuracy as the only success criterion and highlights the need for further fraud-focused optimization.

---

🎯 Threshold Analysis

The project also explores classification threshold optimization.

Instead of relying only on the default classification threshold, different thresholds can be analyzed to understand the trade-off between:

Precision  ↔  Recall

This is particularly important in financial fraud detection, where organizations may prefer higher Recall to detect more suspicious transactions, depending on the acceptable False Positive rate.

---

🧪 Unseen Transaction Prediction

The trained model is also used to demonstrate prediction on an unseen transaction.

Prediction Workflow

New Transaction
       ↓
Data Preprocessing
       ↓
Feature Transformation
       ↓
Trained ML Model
       ↓
Prediction
       ↓
Legitimate / Fraudulent

This demonstrates how a trained model can be applied to new transaction data after the required preprocessing steps.

---

💾 Model Saving

The project includes model persistence using Joblib.

Saving the trained model allows it to be reused later without retraining the complete Machine Learning pipeline from the beginning.

This also provides a foundation for future deployment.

---

🛠️ Technologies & Tools

Programming Language

🐍 Python

Libraries

- Pandas — Data manipulation and analysis
- NumPy — Numerical computing
- Matplotlib — Data visualization
- Seaborn — Statistical visualization
- Scikit-learn — Machine Learning and model evaluation
- Joblib — Model persistence

Concepts

- Data Analytics
- Exploratory Data Analysis
- Data Preprocessing
- Feature Engineering
- Classification
- Predictive Analytics
- Machine Learning
- Model Evaluation
- Fraud Detection
- Data Visualization
- Threshold Optimization

---

📁 Repository Structure

AI_FINANCIAL_FRAUD_DETECTION-REAL_DATASET.IPYNB
│
├── 📓 AI_Financial_Fraud_Detection(Real_Dataset).ipynb
│
├── 📊 Bank_Transaction_Fraud_Detection_part1.csv
│
└── 📄 README.md

Dataset Note

The original dataset is larger than GitHub's individual file-size limit. Therefore, the dataset was prepared into smaller parts for repository storage.

The notebook expects the dataset under the filename:

Bank_Transaction_Fraud_Detection.csv

If the dataset is stored as multiple parts, the parts need to be reconstructed into the expected CSV before running the notebook.

---

🚀 How to Run the Project

1️⃣ Clone the Repository

git clone https://github.com/shaktit159-Analyst/AI_FINANCIAL_FRAUD_DETECTION-REAL_DATASET.IPYNB.git

2️⃣ Open the Notebook

Open:

AI_Financial_Fraud_Detection(Real_Dataset).ipynb

You can run it using:

- Google Colab
- Jupyter Notebook
- JupyterLab

3️⃣ Install Required Libraries

pip install pandas numpy matplotlib seaborn scikit-learn joblib

4️⃣ Prepare the Dataset

Place the complete dataset in the notebook's working directory using the expected filename:

Bank_Transaction_Fraud_Detection.csv

5️⃣ Run the Notebook

Execute the notebook cells sequentially from data loading through model evaluation and prediction.

---

💼 Business Value

This project demonstrates how Machine Learning can support financial organizations in:

🚨 Fraud Monitoring

Identify potentially suspicious transactions using historical transaction patterns.

📊 Risk Analysis

Analyze transaction characteristics associated with fraudulent activity.

🛡️ Customer Protection

Support stronger transaction monitoring and fraud prevention strategies.

⚙️ Automated Analysis

Reduce dependency on purely manual transaction analysis.

📈 Data-Driven Decision Making

Use analytical and predictive techniques to support financial risk management.

---

⚠️ Current Limitations

The current model demonstrates the complete Machine Learning workflow but still has limitations for production-level fraud detection.

The most important limitation is the low fraud Recall observed in the final evaluation.

Additional improvements are therefore required before considering the model suitable for real-time production deployment.

---

🔮 Future Improvements

The project can be further improved through:

- ⚡ Real-time transaction monitoring
- 🚨 Real-time fraud alerts
- 📈 Fraud risk scoring
- ⚖️ Advanced class-imbalance handling
- 🧠 Advanced ensemble and boosting models
- 🔍 Explainable AI (XAI)
- 🎯 Cost-sensitive learning
- 🌐 REST API deployment using Flask or FastAPI
- ☁️ Cloud deployment
- 📊 Interactive fraud analytics dashboard
- 🔄 Automated model retraining
- 📡 Real-time data pipelines
- 🔐 Privacy-preserving financial analytics

---

🌟 Key Learning Outcomes

Through this project, the following practical skills were demonstrated:

- Real-world data analysis
- Exploratory Data Analysis
- Data preprocessing
- Feature engineering
- Handling categorical variables
- Machine Learning classification
- Imbalanced classification evaluation
- Model comparison
- Threshold analysis
- Performance interpretation
- Model persistence
- Business-oriented analytical thinking

---

👨‍💻 Author

Shakti Singh Tomar

MBA – IBM Business Analytics

Areas of Interest

- 📊 Data Analytics
- 🤖 Machine Learning
- 🧠 Artificial Intelligence
- 📈 Predictive Analytics
- 💼 Business Intelligence

---

⭐ Support the Project

If you find this project useful or interesting, consider giving the repository a ⭐ on GitHub.

Feedback and suggestions are always welcome.

---

🔗 Repository

AI Financial Fraud Detection – Real Dataset

https://github.com/shaktit159-Analyst/AI_FINANCIAL_FRAUD_DETECTION-REAL_DATASET.IPYNB

---

<p align="center">🚀 Built with Python • Machine Learning • Predictive Analytics • Data Visualization

Turning financial transaction data into actionable fraud detection insights.

</p>
