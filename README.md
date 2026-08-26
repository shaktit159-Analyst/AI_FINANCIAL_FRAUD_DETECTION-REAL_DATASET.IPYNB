🔐 AI Financial Fraud Detection

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Data%20Analysis-Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-2EA44F?style=for-the-badge)

🚨 AI-Powered Financial Fraud Detection Using Machine Learning

«Turning Financial Transaction Data into Actionable Fraud Detection Insights»

---

🧠 About the Project

AI Financial Fraud Detection is an end-to-end Machine Learning project designed to identify potentially fraudulent financial transactions.

The project works with a 200,000-record financial transaction dataset containing 24 features and demonstrates the complete journey from data analysis and preprocessing to Machine Learning-based fraud prediction.

Complete workflow:

Data Analysis → Data Cleaning → EDA → Feature Engineering → Model Training → Model Evaluation → Threshold Analysis → Fraud Prediction → Model Saving

The project also highlights an important real-world challenge in financial fraud detection: class imbalance and the trade-off between Precision, Recall, False Positives, and False Negatives.

---

🎯 Business Problem

Financial institutions process a huge number of transactions every day. Detecting fraudulent activity quickly and accurately is critical for:

- 🛡️ Customer protection
- 💰 Financial risk reduction
- 🚨 Fraud monitoring
- 📊 Better decision-making
- ⚙️ Automated transaction analysis

Main Question

«Can Machine Learning learn transaction patterns and identify potentially fraudulent transactions?»

---

🎯 Project Objectives

- 🔍 Analyze financial transaction behavior
- 🧹 Clean and preprocess transaction data
- 📊 Perform Exploratory Data Analysis
- 🚨 Identify patterns related to fraudulent transactions
- ⚖️ Understand class imbalance
- 🛠️ Prepare features for Machine Learning
- 🤖 Train multiple classification models
- 📈 Compare model performance
- 🎯 Analyze classification thresholds
- 🧪 Predict an unseen transaction
- 💾 Save the trained model

---

🔄 End-to-End Machine Learning Workflow

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
            ↓
     Final Conclusion

---

📊 Dataset

The project uses a financial transaction dataset containing:

Property| Details
📌 Records| 200,000
📌 Features| 24
🎯 Target Variable| "Is_Fraud"
🧠 Problem Type| Binary Classification
🏦 Domain| Financial / Banking
⚠️ Main Challenge| Class Imbalance

Target Variable

"Is_Fraud"

Value| Meaning
"0"| Legitimate Transaction
"1"| Fraudulent Transaction

---

🔎 Dataset Features

The dataset contains customer, banking, transaction, merchant, device, and location-related information.

👤 Customer Information

- Customer ID
- Customer Name
- Gender
- Age
- State
- City

🏦 Banking Information

- Bank Branch
- Account Type
- Account Balance

💳 Transaction Information

- Transaction ID
- Transaction Date
- Merchant Category
- Transaction Device
- Transaction Location
- Transaction Currency
- Transaction Description

📱 Device & Contact Information

- Device Type
- Customer Contact
- Customer Email

🎯 Target

- "Is_Fraud"

---

🧹 Data Preprocessing

Before training the Machine Learning models, the dataset goes through several preprocessing stages.

Preprocessing Steps

- Data inspection
- Data type analysis
- Missing-value analysis
- Duplicate analysis
- Feature selection
- Numerical feature processing
- Categorical feature encoding
- Feature scaling
- Train-test splitting
- Feature transformation

Scikit-learn Components

StandardScaler
      +
OneHotEncoder
      +
ColumnTransformer
      +
Pipeline

---

📈 Exploratory Data Analysis

Exploratory Data Analysis is performed to understand transaction behavior and identify patterns associated with fraudulent activity.

Key Analysis

- 📊 Fraud vs. legitimate transaction distribution
- 👥 Customer demographics
- 🏦 Account types
- 💳 Transaction behavior
- 🛒 Merchant categories
- 📍 Transaction locations
- 📱 Device types
- 📈 Numerical feature relationships
- 🔗 Correlation analysis
- ⚖️ Class distribution

Visualizations are used to transform raw transaction data into meaningful analytical insights.

---

🤖 Machine Learning Models

Three classification algorithms are trained and compared.

1️⃣ Logistic Regression

Used as a baseline classification model to establish an initial benchmark.

Key characteristics

- Simple and interpretable
- Fast to train
- Useful baseline model

---

2️⃣ Decision Tree Classifier

A tree-based classification algorithm capable of learning non-linear relationships between transaction features.

Key characteristics

- Easy to interpret
- Captures non-linear patterns
- Suitable for classification tasks

---

3️⃣ Random Forest Classifier

An ensemble learning algorithm that combines multiple decision trees.

Key characteristics

- Handles complex relationships
- More robust than a single decision tree
- Suitable for structured transaction data

---

📊 Model Evaluation

Financial fraud detection is an imbalanced classification problem, so Accuracy alone cannot provide a complete picture of model performance.

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

Measures the model's ability to distinguish between fraudulent and legitimate transactions across different thresholds.

PR-AUC

Provides additional insight for imbalanced classification by focusing on the Precision-Recall relationship.

Confusion Matrix

Analyzes:

True Positive
True Negative
False Positive
False Negative

---

⚠️ Important Model Insight

One of the most important findings from this project is:

«High Accuracy does not automatically mean effective fraud detection.»

The final Random Forest evaluation achieved approximately:

Metric| Result
Accuracy| 94.79%
Precision| 5.33%
Recall| 0.20%
F1-Score| 0.38%

🧠 Interpretation

The high Accuracy is influenced by the imbalanced nature of the dataset.

However, the very low Recall indicates that the current model is not yet effective enough at identifying actual fraudulent transactions.

This is an important business insight because missing an actual fraudulent transaction can be costly.

Therefore, the project demonstrates that fraud detection models should not be judged by Accuracy alone.

---

🎯 Threshold Analysis

The project also explores classification thresholds to understand the relationship between:

Precision  ↔  Recall

Changing the classification threshold can affect how aggressively the model flags transactions as potentially fraudulent.

This is important in financial applications because organizations need to balance:

- False Positives
- False Negatives
- Investigation costs
- Customer experience
- Financial risk

---

🧪 Unseen Transaction Prediction

The project demonstrates how the trained Machine Learning model can be applied to an unseen transaction.

Prediction Pipeline

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

This demonstrates the practical use of the trained model beyond the original training data.

---

💾 Model Persistence

The project uses Joblib for saving the trained Machine Learning model.

Benefits

- Reuse the trained model
- Avoid unnecessary retraining
- Prepare the model for future deployment
- Support future API or application integration

---

🛠️ Technology Stack

👨‍💻 Programming Language

Python

📚 Libraries

Technology| Purpose
🐼 Pandas| Data Analysis
🔢 NumPy| Numerical Computing
📊 Matplotlib| Data Visualization
📈 Seaborn| Statistical Visualization
🤖 Scikit-learn| Machine Learning
💾 Joblib| Model Persistence

🧠 Core Concepts

- Machine Learning
- Data Analytics
- Predictive Analytics
- Exploratory Data Analysis
- Data Preprocessing
- Feature Engineering
- Classification
- Imbalanced Classification
- Model Evaluation
- Threshold Analysis
- Fraud Detection
- Data Visualization
- Model Persistence

---

📁 Repository Structure

AI_FINANCIAL_FRAUD_DETECTION-REAL_DATASET.IPYNB
│
├── 📓 AI_Financial_Fraud_Detection(Real_Dataset).ipynb
│
├── 📊 Bank_Transaction_Fraud_Detection_part1.csv
│
└── 📄 README.md

---

📌 Dataset Upload Note

The original dataset is larger than GitHub's individual file-size limit.

Therefore, a smaller repository-compatible dataset file has been prepared for GitHub upload:

Bank_Transaction_Fraud_Detection_part1.csv

⚠️ Important

The notebook expects the complete dataset using the filename:

Bank_Transaction_Fraud_Detection.csv

For complete notebook execution, the complete dataset should be available locally using the expected filename.

---

🚀 How to Run

1️⃣ Clone the Repository

git clone https://github.com/shaktit159-Analyst/AI_FINANCIAL_FRAUD_DETECTION-REAL_DATASET.IPYNB.git

2️⃣ Open the Notebook

AI_Financial_Fraud_Detection(Real_Dataset).ipynb

You can use:

- Google Colab
- Jupyter Notebook
- JupyterLab

3️⃣ Install Dependencies

pip install pandas numpy matplotlib seaborn scikit-learn joblib

4️⃣ Prepare the Dataset

Place the complete dataset in the notebook's working directory:

Bank_Transaction_Fraud_Detection.csv

5️⃣ Run the Notebook

Execute the notebook cells sequentially from:

Data Loading
      ↓
EDA
      ↓
Preprocessing
      ↓
Model Training
      ↓
Model Evaluation
      ↓
Threshold Analysis
      ↓
Prediction

---

💼 Business Value

This project demonstrates how Machine Learning can support financial organizations in:

🚨 Fraud Monitoring

Identify potentially suspicious transactions using historical transaction patterns.

📊 Risk Analysis

Understand transaction characteristics associated with fraudulent behavior.

🛡️ Customer Protection

Support stronger transaction monitoring and fraud prevention strategies.

⚙️ Automated Analysis

Assist financial teams in analyzing large volumes of transaction data.

📈 Data-Driven Decision Making

Use predictive analytics to support financial risk management.

---

⚠️ Current Limitations

The current project demonstrates a complete Machine Learning workflow, but the model should not be considered production-ready.

The most important limitation is the low fraud-detection Recall observed during evaluation.

Before real-world deployment, additional work would be required in areas such as:

- Advanced class-imbalance handling
- Feature engineering
- Hyperparameter optimization
- Advanced Machine Learning algorithms
- Cost-sensitive learning
- Threshold optimization
- Extensive validation
- Real-world transaction testing

---

🔮 Future Scope

The project can be extended into a production-oriented financial fraud detection platform.

🚀 Potential Enhancements

- ⚡ Real-time fraud detection
- 🚨 Automated fraud alerts
- 📈 Fraud risk scoring
- ⚖️ Advanced class-imbalance techniques
- 🧠 XGBoost / LightGBM / advanced ensemble models
- 🔍 Explainable AI (XAI)
- 🎯 Cost-sensitive learning
- 🌐 Flask / FastAPI deployment
- ☁️ Cloud deployment
- 📊 Interactive fraud analytics dashboard
- 🔄 Automated model retraining
- 📡 Real-time transaction streaming
- 🔐 Privacy-preserving financial analytics

---

🌟 Key Learning Outcomes

This project demonstrates practical experience in:

- ✅ Financial Data Analysis
- ✅ Exploratory Data Analysis
- ✅ Data Cleaning
- ✅ Feature Engineering
- ✅ Categorical Encoding
- ✅ Feature Scaling
- ✅ Machine Learning Classification
- ✅ Imbalanced Classification
- ✅ Model Comparison
- ✅ Model Evaluation
- ✅ Threshold Analysis
- ✅ Fraud Prediction
- ✅ Model Persistence
- ✅ Business-Oriented Analytics

---

👨‍💻 Author

Shakti Singh Tomar

🎓 MBA – IBM Business Analytics

Areas of Interest

📊 Data Analytics
🤖 Machine Learning
🧠 Artificial Intelligence
📈 Predictive Analytics
💼 Business Intelligence

---

⭐ Support the Project

If you find this project useful or interesting, consider giving the repository a ⭐.

Your feedback and suggestions are always welcome.

---

🔗 Project

AI Financial Fraud Detection – Real Dataset

GitHub Repository:
"AI_FINANCIAL_FRAUD_DETECTION-REAL_DATASET.IPYNB"

---

<p align="center">🚀 Built with Python • Machine Learning • Predictive Analytics

Turning Financial Transaction Data into Actionable Fraud Detection Insights.

</p>
