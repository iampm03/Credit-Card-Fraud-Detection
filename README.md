# Credit-Card-Fraud-Detection
# Problem Statement

- The problem statement chosen for this project is to predict fraudulent credit card transactions with the help of machine learning models.

# Business Problem Overview

- Retaining highly profitable clients is the primary business objective for many banks. For some banks, however, this objective is seriously threatened by banking fraud. Regarding significant monetary losses, credibility, and trust, this is a worry for banks as well as customers.


- According to the Nilson Report, banking scams are expected to cause 30 billion in losses globally by 2020. New and varied methods of fraudulent transactions are being committed as digital payment channels proliferate.


- Machine learning-based credit card fraud detection is not only popular but also required in the banking sector to implement proactive monitoring and fraud prevention measures. These organizations are benefiting from machine learning by having less time-consuming manual reviews, expensive chargebacks and fees, and denials of valid transactions.


# Understanding and Defining Fraud Logic

Credit card fraud is any dishonest act or behavior to obtain information without proper authorization from the account holder for financial gain. Among different ways of committing frauds, skimming is the most common one, which is a way of duplicating information located on the magnetic strip of the card. Apart from this, following are the other ways:

- Manipulation/alteration of genuine cards
- Creation of counterfeit cards
- Stealing/loss of credit cards
- Fraudulent telemarketing

# About the Dataset

- The data set is taken from the Kaggle website and has a total of 2,84,807 transactions; out of these, 492 are fraudulent. Since the data set is highly imbalanced, it needs to be handled before model building.


- It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.


- The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced; the positive class (frauds) accounts for 0.172% of all transactions.


- It contains only numerical input variables resulting from a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA; the only features not transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction amount, which can be used for example-dependent cost-sensitive learning. Feature 'Class' is the response variable and takes value 1 in case of fraud and 0 otherwise.


- Given the class imbalance ratio, we recommend measuring accuracy using the Area Under the Precision-Recall Curve (AUPRC). The confusion matrix accuracy is not meaningful for unbalanced classification.


# Metric Used

### ROC-AUC Score

- One often used metric to assess the effectiveness of binary classifiers is the ROC-AUC (Receiver Operating Characteristic - Area Under the Curve) score. By computing the area under the receiver operating characteristic curve's curve, a model's capacity to discriminate between positive and negative classes is evaluated.


- Because the ROC-AUC score is insensitive to class imbalance, it can be a useful tool for imbalanced datasets. Thus, even in cases when the dataset's positive and negative classes are unbalanced, the ROC-AUC score will continue to offer a trustworthy indicator of the model's capacity to distinguish between the two classes.


### F1 Score

- It's crucial to remember that the ROC-AUC score does not reveal details about the model's precise performance for every class. The model might perform well in the larger class but poorly in the smaller class, for instance, if one class is noticeably smaller than the other. The ROC-AUC score might not show this. Therefore, while assessing a model's performance on imbalanced datasets, it's crucial to take into account additional metrics like accuracy, recall, F1-score, or confusion matrix.


- A popular metric for assessing the effectiveness of binary classifiers is the F1-score. It gives a measure of the overall accuracy of the model by combining recall and precision into a single score.


### Precision

- A classification or prediction model's precision is a gauge of its accuracy. It can be defined as the ratio in the model's output between the number of true positives (positive cases successfully predicted) and the total number of false positives (positive cases wrongly predicted). To put it another way, precision calculates the percentage of positive situations that are actually anticipated to be positive.


- When a model has a high precision, it means that it is highly effective at finding positive cases and that its output contains few false positives. A poor precision, on the other hand, indicates a higher rate of false positives in the model, which may produce inaccurate or misleading findings.


### Recall

- The completeness of a categorization or prediction model is gauged by recall. In the model's output, it is defined as the ratio of true positives (positive cases that were correctly predicted) to the total of true positives and false negatives (positive cases that were missed). Put differently, recall quantifies the percentage of real positive cases that the model accurately recognizes.


- A high recall means that few positive examples are overlooked by the model, demonstrating its excellent ability to recognize positive situations. Conversely, a low recall indicates a larger likelihood of missing positive cases in the model, which may potentially produce inaccurate or deceptive results.
