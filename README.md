# Hackthon_Participation_CategoryClassification
Classify Category of the Problem based on given dataset

This data represents Dataset of a company which is providing OnCall service to customers for various problem categories.
like, Car breakdown, Home repair etc.

There are three different categories of data given in dataset. Dataset is very skewed with 6001, ~300 and ~100 records for three categories respectively.

I performed Data Imputation, Scalling, Correlation Analysis and Feature engineering of Date Columns as per my understanding.

(1) First, I applied Undersampling and achieved 78-80 % accuracy on Training data.
And in second part, I applied Oversampling technique SMOTE and achieved 95-96 % accuracy on Training data.

(2) Added ROC score for Undersampling and Oversampling cases

(3) Added Precision/Recall as Evaluation Metric - as this is the right metric for used Dataset

(4)  tried to apply Abhishek Thakur's technique he has mentioned in his article "Approaching any ML problem"
https://www.linkedin.com/pulse/approaching-almost-any-machine-learning-problem-abhishek-thakur/

(5)  We are having skewed dataset here. with Problem Category count : (1, 6001), (2, 301), (0, 137) I am creating a dataset with undersampling Category 1, and Oversampling Category 0. I want to make a dataset with 300 samples for each Category respectively. And, I want to check how Classifier results come for this Dataset.

(6)  In this Notebook, I am trying to check how logisitc regression with "class_weight=balanced" behaves on dataset. I will take whole dataset and let Logistic regression take care of class imbalanced. First approach listed here is based on my Notebook 4 Data PreProcessing. And, Second approach listed here is based on my Notebook 3 Data Processing. Let us see what happens !!

My Observation says that Logistic Regression and Decision Tree Classifier output shows pretty good improvement while using class_weight='balanced' parameter.
But, Ensemble Learning Classifiers like Decision Forest Classifier and XGBClassifiers' performance is almost unchanged.¶

Any feedback about improving my solution will be appreciated.

Thanks,
Kunjan Shah.
