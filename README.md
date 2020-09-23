# Healthcare Fraud Detection

The primary objective of this project was engineering features to analyze inconsistincies in Provider data, and by extension, 
detect healthcare fraud. 

The data was downloaded from: https://www.kaggle.com/rohitrox/healthcare-provider-fraud-detection-analysis

The data in its original form comprised of eight different csv files. Four of these files were train(labelled data): beneficiary, outpatient, inpatient, 
and flagged fraudulent providers. The remaining four files were test(unlabelled data): beneficiary, outpatient, inpatient, and providers.

One of the greatest tasks in this project was to create a usable data frame. The beneficiary, outpatient, and inpatient datasets were at the level
of the patients and claims, whereas the target data (flagged fraudulent providers) for the labelled dataset was at the level of the providers. Therefore, 
we had to aggregate and transform inpatient, outpatient, and beneficiary data to create a new dataset based on the providers. 

The Team folder contains code for: 
* EDA - Exploratory Data Analysis 
* Feature_Engineering Train - All of the features engineered based on provider for labelled (train) dataset
* Feature_Engineering Test - All of the features engineered based on provider for unlabelled (test) dataset
* Powerpoint Graphs - Feature Engineering Sections - contains Extra Trees Classifier, Lasso Regression for Feature Importance, and Penalized Logistic Regression
* MachineLearningModels(supervised) - contains all of the supervised machine learning models performed on labelled dataset
* K-Means Clustering - Unsupervised K-Means clustering on the unlabelled dataset and data analysis using appended K labels
* Market Basket Analysis - MBA done on chronic conditions 
