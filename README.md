# DATASTORM-KOALACODERS
IMPORTANT NOTES
**DAY 1**

We mainly focused on basic feature enginerring and extensive model selection and training process
After some extensive searching we finalised Multiple random forests with feature splitting and XGBoost are good models to tain our imbalanced data( We upsampled the minority class using SMOTE algorithm)
**Multiple random forests with feature splitting**
on the first hand we didnt dive into extensive feature eng process but we did seperated numerical and cateogarical data. We created a transformation pipeline to standard scale numerical data and onehotencode cateogarical data.then our motive was to use multiple random forests and train them by splitting the features into groups and we assumed that this will improve the cross validation accuracy. In this case, we have used two random forest classifiers, and we trained them with different sets of features. Next using the results of these two random forest and all of the initial features, another random forest was trained to get the final result. All together there were three random forests working together to predict the revenues.
**XGBoost**
on the first hand we didnt dive into extensive feature eng process but we did seperated numerical and cateogarical data. We created a transformation pipeline to standard scale numerical data and onehotencode cateogarical data.
We chose to use XGBoost because:

XGBoost is an extreme gradient boosting algorithm based on trees that tends to perform very well out of the box compared to other ML algorithms.
XGBoost is popular with data scientists and is one of the most common ML algorithms used in Kaggle Competitions.
XGBoost allows you to tune various parameters.
XGBoost allows parallel processing.

**BEST MODEL OF DAY 1- Upsampled data & XGBoost**

**DAY 3**
After getting moderate success during day 1, our focus turned towards extensive **FEATURE ENGINEERING** in bid for higher F1 score.
//FEATURE ENGINEERING TECHNIQUES USED**
1.Feature selection using pearson's coefficients
2.Feature selection using linear models
3.Feature extraction using PCA.
4.Tranformation pieline to standard scale numerical data and to onehot encode cateogarical data

Then we trained each and every outcome with Multiple random forests with feature splitting and XGBoost.

**BEST MODEL OF DAY 3- Feature selection using linear models and XGBoost**
