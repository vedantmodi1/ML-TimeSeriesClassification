# ML-TimeSeriesClassification

Tasks Performed:
Data Preparation:

Conducted minor data cleaning.
Extracted various time-domain features (e.g., minimum, maximum, mean, median, standard deviation, quartiles) from six time series per instance.
Estimated standard deviations of these features and built 90% bootstrap confidence intervals using Python's bootstrapped method.
Feature Selection:

Identified the three most important time-domain features for subsequent classification tasks.
Binary and Multiclass Classification:

Binary Classification (Logistic Regression):

Classified bending vs. other activities using logistic regression.
Visualized scatter plots of selected features to distinguish activities.
Split each time series into two parts, doubling the feature set for analysis.
Employed logistic regression with varying segmentations of time series.
Used recursive feature elimination (RFE) with cross-validation to optimize feature selection.
Addressed class imbalance with stratified cross-validation.
Reported classifier performance metrics (confusion matrix, ROC curve, AUC score) on training and test sets.
Adjusted logistic regression for class imbalance and instability in parameter estimation.
Binary Classification (L1-penalized Logistic Regression):

Repeated binary classification using L1-penalized logistic regression, replacing p-value selection with L1 regularization.
Cross-validated for optimal parameters (number of time series segments, regularization weight).
Multiclass Classification (Naïve Bayes' Classifier):

Extended classification to all activities using Naïve Bayes' classifier with Gaussian and Multinomial priors.
Compared performance metrics (AUC, test error) across different classifier types and priors.

Palumbo,Filippo, Gallicchio,Claudio, Pucci,Rita, and Micheli,Alessio. (2016). Activity Recognition system based on Multisensor data fusion (AReM). UCI Machine Learning Repository. https://doi.org/10.24432/C5SS33.
