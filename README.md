# Credit-Card-Fraud-Detection
An end-to-end Credit Card Fraud Detection project built using a Kaggle dataset. Includes data preprocessing, exploratory data analysis (EDA), visualization Logistic Regression, and a Random Forest classifier to identify fraudulent transactions and enhance financial risk management

# Dataset
Source: Kaggle - Credit Card : https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
Records: 284,807 transactions
Features: 30 numerical variables (V1-V28 are PCA components, plus Time, Amount, and Class)
Fraud Ratio: Only 0.17% of transactions are fraudulent

# Technologies Used
Language: Python
Libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
Models: Logistic Regression, Random Forest Classifier

# Exploratory Data Analysis (EDA)
Identified severe class imbalance
Visualized distribution of Amount, Time, and anonymized features
Used correlation matrix and boxplots to detect potential fraud patterns
Found distinct transaction behavior in fraud vs. non-fraud cases

# Data Preprocessing
Scaled Amount and Time using StandardScaler
Performed train-test split (70:30 ratio)
Used undersampling to balance classes
Removed outliers and normalized features

# Models & Results
✅ Logistic Regression
Precision (fraud class): 83%
Recall (fraud class): 63%
F1 Score: 0.72
ROC AUC: 0.958

✅ Random Forest Classifier
Outperformed logistic regression in recall and AUC
Handled class imbalance better and provided stronger generalization

# Evaluation Metrics
Confusion Matrix
TP: 62, FN: 36, TN: 56851, FP: 13 (Logistic Regression)
Classification Report
Balanced accuracy and precision-recall tradeoff
ROC Curve
AUC of ~0.96 indicates strong separability

📌 Key Insights
Fraudulent transactions have distinct patterns in feature distribution
Imbalanced data requires careful handling for effective fraud detection
Random Forest offers better recall and robustness than Logistic Regression

💼 Business Impact
Detecting fraud early helps financial institutions save millions
Improves customer trust and reduces operational risk
Supports regulatory compliance and customer satisfaction
