
# Credit Card Fraud Detection Project


## Objective

This project aims to implement various methodologies to detect credit card fraud using highly imbalanced data. The dataset has undergone Principal Component Analysis (PCA) for anonymization purposes. Three different analyses were conducted: one without any sampling, the second using undersampling (RandomSampler), and the third using SMOTE for oversampling.
## Methodologies Implemented
1.No Sampling: Analyzed using five different algorithms (Gradient Boosting, Random Forest, Decision Tree, SVM, Neural Network). \
2.Undersampling: Applied RandomSampler to balance the data before analysis. \
3.Oversampling: Employed SMOTE to oversample the minority class for better model performance.
## Strategy
My solution to solve this problem will be the development of a data science project. This project will have a machine learning model which can predict whether a transaction is fraudulent or not.

Step 01. Data Description: In this first section the data will be collected and studied. The missing values will be threated or removed. Finally, a initial data description will carried out to know the data. Therefore some calculations of descriptive statistics will be made, such as kurtosis, skewness, media, fashion, median and standard desviation.

Step 02. Feature Engineering: In this section, a mind map will be created to assist the creation of the hypothesis and the creation of new features. These assumptions will help in exploratory data analysis and may improve the model scores.

Step 03. Data Filtering: Data filtering is used to remove columns or rows that are not part of the business. For example, columns with customer ID, hash code or rows with age that does not consist of human age.

Step 04. Exploratory Data Analysis: The exploratory data analysis section consists of univariate analysis, bivariate analysis and multivariate analysis to assist in understanding of the database. The hypothesis created in step 02 will be tested in the bivariate analysis.

Step 05. Data Preparation: In this fifth section, the data will be prepared for machine learning modeling. Therefore, they will be transformed to improve the learning of the machine learning model, thus they can be encoded, oversampled, subsampled or rescaled.

Step 06. Feature Selection: After the data preparation in this section algorithms, select the best columns to be used for the training of the machine learning model. This reduces the dimensionality of the database and decreases the chances of overfiting.

Step 07. Machine Learning Modeling: Step 07 aims to train the machine learning algorithms and how they can predict the data. For validation the model is trained, validated and applied to cross validation to know the learning capacity of the model.

Step 08. Hyparameter Fine Tuning: Firstly selected the best model to be applied in the project, it's important to make a fine tuning of the parameters to improve its scores. The same model performance methods apllied in the step 07 are used.

Step 09. Conclusions: This is a conclusion stage which the generation capacity model is tested using unseen data. In addition, some business questions are answered to show the applicability of the model in the business context.

## Results Summary
### No Sampling Metrics

#### Gradient Boosting:

Accuracy: 99.83% Precision: 52.94% Recall: 18.37% F1 Score: 27.27%

#### Random Forest:

Accuracy: 99.96% Precision: 94.12% Recall: 81.63% F1 Score: 87.43%

#### Decision Tree:

Accuracy: 99.92% Precision: 76.70% Recall: 80.61% F1 Score: 78.61%

#### SVM:

Accuracy: 99.93% Precision: 77.67% Recall: 81.63% F1 Score: 79.60%

#### Neural Network:

Accuracy: 99.92% Precision: 76.70% Recall: 80.61% F1 Score: 78.61%

### Undersampling Metrics

#### Gradient Boosting:

Accuracy: 95.94% Precision: 96.88% Recall: 94.90% F1 Score: 95.88%

#### Random Forest:

Accuracy: 95.43% Precision: 96.84% Recall: 93.88% F1 Score: 95.34%

#### Decision Tree:

Accuracy: 89.85% Precision: 86.79% Recall: 93.88% F1 Score: 90.20%

#### SVM:

Accuracy: 95.43% Precision: 100.00% Recall: 90.82% F1 Score: 95.19%

#### Neural Network:

Accuracy: 96.45% Precision: 100.00% Recall: 92.86% F1 Score: 96.30%

### Oversampling Metrics

#### Gradient Boosting:

Accuracy: 97.79% Precision: 98.57% Recall: 96.99% F1 Score: 97.77%

#### Random Forest:

Accuracy: 99.99% Precision: 99.97% Recall: 100.00% F1 Score: 99.99%

#### Decision Tree:

Accuracy: 99.80% Precision: 99.73% Recall: 99.88% F1 Score: 99.80%

#### SVM:

Accuracy: 96.52% Precision: 98.27% Recall: 94.71% F1 Score: 96.46%

#### Neural Network:

Accuracy: 99.54% Precision: 99.08% Recall: 100.00% F1 Score: 99.54%
## Analysis and Insights
1. No Sampling: Models show high accuracy but struggle with recall, indicating challenges in detecting fraud cases. 
2. Undersampling: Improved recall but at the expense of precision. Some models display better recall but compromised precision. 
3. versampling: Achieved superior recall without compromising precision. Neural Network stands out with perfect recall.
## Confusion Matrix Analysis
1. Oversampling: Neural Network excelled by never misclassifying fraud as non-fraud, crucial for this project's objective. 

2. ROC Curve: An AUC (Area Under the ROC Curve) value of 0.89 indicates a relatively good performance of the model in distinguishing between the classes in a binary classification problem.

AUC values range between 0 and 1, with 1 being a perfect classifier that perfectly separates the classes. An AUC of 0.89 suggests that the model's predictions are quite good, significantly better than random guessing, as a random classifier would have an AUC of 0.5. Generally, the interpretation of AUC values can be as follows:

AUC around 0.5: The model's performance is similar to random guessing. AUC between 0.5 and 0.7: The model's performance is poor to fair. AUC between 0.7 and 0.9: The model's performance is good. AUC above 0.9: The model's performance is excellent. An AUC of 0.89 indicates that the model has a strong ability to discriminate between positive and negative classes, although the interpretation might slightly vary depending on the specific context of the problem and the domain. Overall, an AUC of 0.89 is considered a quite good performance for a binary classification model.
## Conclusion
The analysis highlights the trade-offs between different sampling techniques. Oversampling, particularly with the Neural Network model, demonstrates promising results, achieving high recall without compromising precision—a crucial aspect in fraud detection scenarios.