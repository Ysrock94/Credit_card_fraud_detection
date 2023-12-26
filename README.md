                                     Credit Card Fraud Detection Project
**Overview**
This project aims to implement various methodologies to detect credit card fraud using highly imbalanced data. The dataset has undergone Principal Component Analysis (PCA) for anonymization purposes. Three different analyses were conducted: one without any sampling, the second using undersampling (RandomSampler), and the third using SMOTE for oversampling.

**Methodologies Implemented**
1.No Sampling: Analyzed using five different algorithms (Gradient Boosting, Random Forest, Decision Tree, SVM, Neural Network).
2.Undersampling: Applied RandomSampler to balance the data before analysis.
3.Oversampling: Employed SMOTE to oversample the minority class for better model performance.

**Results Summary**

**No Sampling Metrics**

**Gradient Boosting:**

Accuracy: 99.83%
Precision: 52.94%
Recall: 18.37%
F1 Score: 27.27%

**Random Forest:**

Accuracy: 99.96%
Precision: 94.12%
Recall: 81.63%
F1 Score: 87.43%

**Decision Tree:**

Accuracy: 99.92%
Precision: 76.70%
Recall: 80.61%
F1 Score: 78.61%

**SVM:**

Accuracy: 99.93%
Precision: 77.67%
Recall: 81.63%
F1 Score: 79.60%

**Neural Network:**

Accuracy: 99.92%
Precision: 76.70%
Recall: 80.61%
F1 Score: 78.61%
Undersampling Metrics

**Gradient Boosting:**

Accuracy: 95.94%
Precision: 96.88%
Recall: 94.90%
F1 Score: 95.88%

**Random Forest:**

Accuracy: 95.43%
Precision: 96.84%
Recall: 93.88%
F1 Score: 95.34%

**Decision Tree:**

Accuracy: 89.85%
Precision: 86.79%
Recall: 93.88%
F1 Score: 90.20%

**SVM:**

Accuracy: 95.43%
Precision: 100.00%
Recall: 90.82%
F1 Score: 95.19%

**Neural Network:**

Accuracy: 96.45%
Precision: 100.00%
Recall: 92.86%
F1 Score: 96.30%

**Oversampling Metrics**

**Gradient Boosting:**

Accuracy: 97.79%
Precision: 98.57%
Recall: 96.99%
F1 Score: 97.77%

**Random Forest:**

Accuracy: 99.99%
Precision: 99.97%
Recall: 100.00%
F1 Score: 99.99%

**Decision Tree:**

Accuracy: 99.80%
Precision: 99.73%
Recall: 99.88%
F1 Score: 99.80%

**SVM:**

Accuracy: 96.52%
Precision: 98.27%
Recall: 94.71%
F1 Score: 96.46%

**Neural Network:**

Accuracy: 99.54%
Precision: 99.08%
Recall: 100.00%
F1 Score: 99.54%

**Analysis and Insights**

1.No Sampling: Models show high accuracy but struggle with recall, indicating challenges in detecting fraud cases.
2.Undersampling: Improved recall but at the expense of precision. Some models display better recall but compromised precision.
O3.versampling: Achieved superior recall without compromising precision. Neural Network stands out with perfect recall.

**Confusion Matrix Analysis**

1.Oversampling: Neural Network excelled by never misclassifying fraud as non-fraud, crucial for this project's objective.
2.ROC Curve: An AUC (Area Under the ROC Curve) value of 0.89 indicates a relatively good performance of the model in distinguishing between the classes in a binary classification problem.

AUC values range between 0 and 1, with 1 being a perfect classifier that perfectly separates the classes.
An AUC of 0.89 suggests that the model's predictions are quite good, significantly better than random guessing, as a random classifier would have an AUC of 0.5.
Generally, the interpretation of AUC values can be as follows:

AUC around 0.5: The model's performance is similar to random guessing.
AUC between 0.5 and 0.7: The model's performance is poor to fair.
AUC between 0.7 and 0.9: The model's performance is good.
AUC above 0.9: The model's performance is excellent.
An AUC of 0.89 indicates that the model has a strong ability to discriminate between positive and negative classes, although the interpretation might slightly vary depending on the specific context of the problem and the domain. Overall, an AUC of 0.89 is considered a quite good performance for a binary classification model.


**Conclusion**

The analysis highlights the trade-offs between different sampling techniques. Oversampling, particularly with the Neural Network model, demonstrates promising results, achieving high recall without compromising precision—a crucial aspect in fraud detection scenarios.
