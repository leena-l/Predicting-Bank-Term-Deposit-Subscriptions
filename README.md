# Bank Marketing Classification using Decision Trees

This project implements a machine learning pipeline to predict customer behavior for a bank’s telemarketing campaign. The goal is to predict if a client will subscribe to a term deposit.

Dataset Overview

The project uses the Bank Marketing Dataset (ID: 222) from the UCI Machine Learning Repository.

Target Variable (y): Binary classification (Yes/No) indicating if the term deposit was subscribed.

Features: Includes customer age, job type, marital status, education, account balance, and campaign details.


# Requirements

To run this project, you need the following Python libraries:

pandas

numpy

matplotlib

seaborn

scikit-learn

ucimlrepo


# Workflow

1 - Data Acquisition

The dataset is fetched directly from the UCI repository using the ucimlrepo library.

2- Preprocessing

Categorical Encoding: Used LabelEncoder to convert categorical text data into numerical format for the model.

Missing Values: Handled the inherent structure of the UCI dataset (noting significant missing values in columns like poutcome and contact).

3 - Model Building

Algorithm: Decision Tree Classifier.

Hyperparameters: max_depth=5 was used to prevent overfitting and ensure the tree remains interpretable.

Data Splitting: 80% training and 20% testing, stratified to maintain class balance.

4 - Evaluation

The model performance is evaluated using:

Accuracy Score: Currently achieving ~89.7%.

Confusion Matrix: Visualized via Seaborn heatmap to see True Positives vs. False Positives.

Classification Report: Detailed breakdown of Precision, Recall, and F1-score for both classes.


# Results

Accuracy: 0.90

Class 0 (No): High precision and recall.

Class 1 (Yes): Lower recall (~0.40), suggesting the model is conservative in predicting successful subscriptions, likely due to class imbalance in the dataset.

# Visualization

The final step includes a high-resolution plot of the Decision Tree, showing the logic paths (splits) based on features like duration, poutcome, and contact.

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page] if you want to contribute.
