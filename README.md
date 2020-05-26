# Knn-Randomforest-Gradientboosting-Classifiers

Exploratory Data Analysis

The first step in the machine learning pipeline is taking a look at the data to make sure that you
understand what you are working with.
Step1: The file was converted into data frame for convenience.

Step2:Segregated the data into continuous numeric data and categorical data.

Step3: Checked if there are any missing values in the given data sets and found there are no missing
values. If there were missing values, then we can handle that by replacing missing values by 'mean' in
features with continuous numeric data and by 'mode' in features with categorical data. There are no
categorical data.

Step4: Couldn't find Unique Identifier Coulmn.

Step5: Checked whether the given datasets are balanced or not, and found the datasets are balanced.

Step6: Found Correlation between Input variables and Target variable. The correlations were not sig-
nificant.


Baseline Models

Formulated 3 baseline models : 1.Random Forest Classier Below are the accuracies before performing
feature engineering and optimizing the model's hyperparameters.
Value of Accuracy train: 0.993000
value of Accuracy test: 0.698333
2.Gradient Boosting Classifier Below are the accuracies before performing feature engineering and opti-
mizing the model's hyperparameters.
value of Accuracy train: 1.000000
value of Accuracy test: 0.840000
3.K-Nearest Neighbors Classifier Below are the accuracies before performing feature engineering and
optimizing the model's hyperparameters.
value of Accuracy train: 0.826500
value of Accuracy test: 0.723333

Feature Engineering

1. Normalization of Data set. It didn't prove much effective in order to improve accuracy of my baseline
models.

2, Used SelectKBest function to select important features, on which I trained and tested the three models.
For Random Forest Classifier and K-Nearest Neighbors Classifier selected 15 best features for maximum
accuracy and for Gradient Boosting Classifier selected 12 features for maximum accuracy.
