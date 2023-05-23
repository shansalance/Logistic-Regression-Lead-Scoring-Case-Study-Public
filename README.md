# Logistic-Regression-Lead-Scoring-Case-Study-Public

Lead Scoring Case Study
This repository contains the code and documentation for the Lead Scoring Case Study conducted for X Education. The objective of this study was to identify the most promising leads that have a high probability of converting into paying customers. The target lead conversion rate set by the CEO was approximately 80%.

Problem Statement
X Education, an online course provider, wanted to improve their lead conversion process. They sought assistance in developing a lead scoring model that could assign a lead score to each potential customer. The goal was to prioritize leads with higher scores, indicating a higher chance of conversion.

Solution Summary
The Lead Scoring Case Study involved the following steps:

Data Analysis and Understanding: The dataset was thoroughly analyzed to gain insights into the variables and their relationships.

Data Cleaning: Variables with a high percentage of missing values were dropped, and missing values were imputed using appropriate methods. Outliers were also identified and treated.

Exploratory Data Analysis (EDA): EDA techniques were applied to understand the data distribution and identify variables with low variability or redundant information.

Creating Dummy Variables: Categorical variables were converted into dummy variables for further analysis.

Test-Train Split: The dataset was split into a training set (70%) and a test set (30%) to train and evaluate the model, respectively.

Feature Rescaling: Numerical variables were rescaled using the Min-Max scaling technique to bring them within a common range.

Feature Selection using Recursive Feature Elimination (RFE): RFE was used to select the top 20 most important features. The significance of the features was determined by examining p-values, and only the most significant features (15 in total) were retained.

Model Development and Evaluation: A statistical model was built using the selected features. The conversion probability for each lead was calculated, assuming a probability cutoff of 0.5. Confusion metrics, including accuracy, sensitivity, and specificity, were calculated to evaluate the overall performance of the model.

ROC Curve Analysis: The Receiver Operating Characteristic (ROC) curve was plotted to assess the model's accuracy and determine the area under the curve (AUC).

Optimal Cutoff Point: By analyzing the accuracy, sensitivity, and specificity for different probability values, an optimal cutoff point of 0.37 was identified. This cutoff point balanced the tradeoff between correctly predicting converted leads and avoiding false positives.

Precision and Recall Metrics: Precision and recall metrics were computed on the train dataset, with precision at 79% and recall at 70.5%. These metrics provided insights into the tradeoff between correctly identifying converted leads and minimizing false positives.

Predictions on the Test Set: The model was applied to the test set to predict the conversion probabilities. The accuracy, sensitivity, and specificity on the test set were calculated as 80.8%, 78.5%, and 82.2% respectively.
