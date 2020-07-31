# Telecom-Churn-Case-Study
Predict the churn in the last (i.e. the ninth) month using the data (features) from the first three months.

# Data Preparation
# Filtering high-value customers/ 
High-value customers are those who have recharged with an amount more than or equal to X, where X is the 70th percentile of the average recharge amount in the first two months (the good phase)./
# Tagging churners and removing attributes of the churn phase/
Now tag the churned customers (churn=1, else 0) based on the fourth month as follows: Those who have not made any calls (either incoming or outgoing) AND have not used mobile internet even once in the churn phase. The attributes used to tag churners are:
total_ic_mou_9/
total_og_mou_9/
vol_2g_mb_9/
vol_3g_mb_9/
After tagging churners, remove all the attributes corresponding to the churn phase

# Steps to build the model
1. Preprocess data (convert columns to appropriate formats, handle missing values, etc.)
2. Conduct appropriate exploratory analysis to extract useful insights (whether directly useful for business or for eventual modelling/feature engineering).
3. Derive new features.
4. Reduce the number of variables using PCA.
5. Train a variety of models, tune model hyperparameters, etc. (handle class imbalance using appropriate techniques).
6. Evaluate the models using appropriate evaluation metrics. As it is more important to identify churners than the non-churners accurately - choosing an appropriate evaluation metric which reflects this business goal is extremely important.
