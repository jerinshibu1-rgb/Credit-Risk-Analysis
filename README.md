# Credit-Risk-Analysis
Project Overview
This project focuses on credit risk analysis using the German Credit Dataset. The goal is to predict whether a loan applicant is a good credit risk or bad credit risk based on financial and personal attributes.
Such models are widely used by banks and financial institutions to reduce default risk and make informed lending decisions.

Dataset Description
 Key Features
Age
Sex
Job
Housing
Saving accounts
Checking account
Credit amount
Duration
Purpose

Target Variable
Risk
Good → Low credit risk
Bad → High credit risk

Importing Libraries
The notebook begins by importing essential Python libraries:
Libraries Used
NumPy & Pandas → Data manipulation
Matplotlib & Seaborn → Data visualization
Scikit-learn →
  Preprocessing
  Model training
  Evaluation metrics
This ensures the workflow follows industry-standard ML practices.

Data Loading & Inspection
You load the dataset and perform initial checks:
Key Steps
Viewing first few rows (head())
Checking dataset shape
Identifying data types
Checking missing values
This step ensures data quality and consistency before modeling.

Exploratory Data Analysis (EDA)
Univariate Analysis
Distribution of credit amount
Age distribution
Loan duration patterns

Categorical Analysis
Credit risk vs:
Housing type
Job category
Purpose of loan

Key Insights
Certain loan purposes have higher default rates
Higher credit amount often correlates with higher risk
Younger applicants show slightly higher risk tendency

EDA helps you understand hidden patterns in customer behavior.

Handling Missing Values
Some columns (like Saving accounts and Checking account) contain missing values.
✔ Solution Used
Filled missing values with:
Mode (most frequent category)
 This preserves dataset size without introducing bias.

   Feature Engineering & Encoding
   Encoding Categorical Variables

Converted categorical features into numerical form using:
Label Encoding
One-Hot Encoding
Why This Is Important
Machine learning models cannot work with text data directly, so encoding is required.

Train-Test Split
The dataset is split into:
Training set → Used to train the model
Testing set → Used to evaluate performance

Common split used:
80% Training
20% Testing

Prevents overfitting and ensures fair evaluation.

Model Building
You experiment with classification models such as:
 Algorithms Used
Logistic Regression
Decision Tree Classifier
Random Forest Classifier
K-Nearest Neighbors (KNN)

Each model is trained using the training data.

 Model Evaluation
 Metrics Used
Accuracy
Confusion Matrix
Classification Report
Precision
Recall
F1-score

Model Comparison & Selection
You compare models based on:
Accuracy
Stability
Ability to handle imbalance

Best Performing Model
 Random Forest / Logistic Regression (depending on your final result)
Chosen due to:
Better generalization
Balanced precision and recall

Final Conclusion
Project Outcomes

Successfully built a credit risk prediction system
Identified important features affecting loan risk
Demonstrated full ML lifecycle:
Data cleaning
EDA
Feature engineering
Modeling
Evaluation

Real-World Impact
This model can help banks:
Reduce loan defaults

Automate decision-making

Improve customer segmentation
