# NLPHotelReview
Table of Contents:
[1] Introduction
Overview of the Objective
[2] Exploratory Data Analysis
Loading and Understanding the Data
Basic Statistical Analysis,Data Visualizations, Key Observations for Actionable Insights
[3] PreProcessing
Text Data Processing for Modeling
Splitting Data into Train and Test Sets
CountVectorizer for Positive and Negative Reviews
Tokenizer and Text Cleaning Steps
Merging Numeric Features with Processed Text Data
[4] Modeling:
Logistic Regression Model by Analyzing Train and Test Accuracy
Identying Top 20 Words and Dra Actionable Insights
[5] In-Depth Model Evaluation:
Confusion Matrix Analysis
Model Errors, Precision, and Recall Metrics
Insights from the Best Performance Model
[6] Conclusion:
Summary of Findings and Recommendations
### Using a pipeline, combine PCA with a decision tree classifier.

Logistic Regression Accuracy: 0.7277908343125734
Decision Tree Accuracy: 0.7198589894242068

ROC-AUC with no sampling -- 0.8381
ROC-AUC with SMOTE -- 0.8666

| |recall|precision|f1|
|-|------|---------|--|
|**logreg on unsampled data**|73.0%|82.3%|0.77%|
|**logreg on SMOTE-sampled data**|81.6%|81.2%|0.81%|


Summary:
Precision-Recall Area Under the Curve is a metric that measures the area under the precision-recall curve. It provides a summary of a model's performance across various levels of precision and recall.
the increase in Precision-Recall Area Under the Curve from 0.87 to 0.89 after applying SMOTE suggests an overall improvement in the model's ability to handle class imbalance, resulting in better recall and precision for the minority class. This is a positive outcome, indicating that SMOTE has contributed to the model's effectiveness in predicting instances of the minority class.

