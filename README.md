# To Oversample or Undersample
An analysis of sampling techniques and their effect on the prediction quality of classification modelling.
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

<img src="https://github.com/ssopic/To_Oversample_or_Undersample/blob/main/cover%20image.png">


Introduction
This repository contains the code and results for an analysis of sampling techniques and their effect on the prediction quality of classification modeling. The analysis compares the performance of different sampling techniques (over-sampling, under-sampling, and a combination of both) on a dataset of employee data. The goal is to identify the best sampling technique for predicting employee attrition.

Data
The dataset used in this analysis is a human resources dataset that contains information on employee demographics, compensation, department, and tenure within the company. The target variable is employee attrition, which is a binary variable indicating whether or not an employee has left the company.

Methods
The analysis was conducted using the following steps:

Data preprocessing: The data was preprocessed to clean and prepare it for analysis. This included removing irrelevant variables, encoding categorical variables, and splitting the data into training and testing sets.
Sampling: Different sampling techniques were applied to the training data to address the class imbalance. The sampling techniques used were:
Random oversampling: This technique creates additional observations for the minority class to balance the dataset.
Random undersampling: This technique removes observations from the majority class to balance the dataset.
Tomek links: This technique removes observations from both the majority and minority classes that are located on the boundaries between the classes.
SMOTE: This technique creates new synthetic observations for the minority class by interpolating between existing minority class observations.
ADASYN: This technique is similar to SMOTE, but it places more emphasis on generating synthetic observations for minority class observations that are located in denser regions of the feature space.

Model training and evaluation: 
Different classification models were trained on the training data and evaluated on the testing data. The models used were:
Logistic regression
Random forest
AdaBoost
Support vector machines
K-nearest neighbors
Decision trees 

The performance of the models was evaluated using the following metrics:
Accuracy
Precision
Recall
AUC

Results
The results of the analysis show that the best sampling technique for predicting employee attrition is SMOTE. The SMOTE technique was able to achieve the highest accuracy, precision, and AUC scores. The other sampling techniques also performed well, but they were not as consistent as SMOTE.

Conclusion
The analysis shows that sampling techniques can have a significant impact on the prediction quality of classification modeling. The best sampling technique for a given dataset will depend on the specific characteristics of the data and the classification model being used. However, SMOTE is a good general-purpose sampling technique that can be used to improve the performance of classification models on imbalanced datasets.
