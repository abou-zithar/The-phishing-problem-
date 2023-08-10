
# Phishing Website Detection using Machine Learning
This README provides an overview of the Python code that performs phishing website detection using machine learning techniques. The aim of this project is to classify websites as legitimate, suspicious, or phishy based on various features.

## Dataset and Problem Description
Phishing websites pose a significant threat to online transactions, especially in the e-banking and e-commerce sectors. The dataset used for this analysis contains 1353 different websites with features related to both legitimate and phishing websites. The attributes include information such as URL Anchor, Request URL, SFH, URL Length, Having '@', Prefix/Suffix, IP, Sub Domain, Web traffic, Domain age, and the final classification label (Legitimate, Suspicious, or Phishy).

## Code Overview
The code performs the following steps:

## Data Loading and Preprocessing
The code starts by importing necessary libraries and loading the dataset using pandas. The dataset is read from a CSV file located in Google Drive. The initial data exploration is performed using pandas functions such as head(), info(), shape, and describe() to get insights about the data.

## Data Visualization
Data visualization is crucial to understanding the distribution of features and their relationships. The code utilizes the Plotly Express library to create a scatter plot to visualize the data points in multi-dimensional space.

Additionally, a heatmap is generated using Seaborn to visualize the correlation between different features.

## Data Preprocessing and Model Building
The dataset is split into features (X) and the target variable (y). Since the dataset is imbalanced, the Synthetic Minority Over-sampling Technique (SMOTE) is applied to balance the classes. The code shows the transformation of class distribution before and after applying SMOTE.

The data is then split into training and testing sets using the train_test_split function. A Naive Bayes classifier (GaussianNB) is chosen for this example. The model is trained using the training data and its accuracy on both training and testing sets is computed using the score() function.

## Conclusion
This README provides a walkthrough of the phishing website detection code, showcasing how machine learning techniques can be used to classify websites into different categories. The code demonstrates data loading, visualization, preprocessing, and model building. Users can further explore different algorithms, perform hyperparameter tuning, and fine-tune the preprocessing steps to improve the model's performance and generalize it to real-world scenarios.
