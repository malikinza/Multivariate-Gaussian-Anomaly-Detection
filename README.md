# Multivariate-Gaussian-Anomaly-Detection

Anomaly/ outlier detection is the identification of rare observations in a dataset. Anomaly detection differs from normal classification in that anomalous datasets are imbalnaced. In this project, I performed anomaly detection on a credit card fraud dataset. The dataset was highly skewed, with only 0.2% fraud cases. Since 99.8% of the dataset fits the non-fraud class, a standard classification algorithm (assume balanced data) would ignore the fraud class and focus on classifying the non-fraud class accurately. 

To detect the fraud cases, I used Multivariate Gaussian to model the data. I plotted the distribution of each feature to identify features with the largest differences in distribution between fraudulent and non-fradulent data. Then, I built an outlier detection model using a Mixture of Gaussians on five features with the largest difference between fradulent and non-fraudlent distributions. Finally, I computed the ROC curve and AUC score to evaluate the model. 

