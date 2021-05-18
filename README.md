# OpenFoodsFact

__Authors:__ Man Chong Chan, Samuel Guo, Gabe Taylor

__Data source:__ https://world.openfoodfacts.org/

__Summary:__ The goal of this project is two-fold: unsupervised and supervised learning on french market food products. The unsupervised task was aimed at extracting meaningful groups of similar ingredients via clustering on the macronutrient profiles of the food products. After obtaining promising results from the unsupervised portion, we turned to the supervised task, which involved both a classification and regression component. Our goal was to reliably predict the nutrition score of a food product given only the list of ingredients and additives. To perform the classification task, we split the target at the median value in effort to separate “healthy” products from “unhealthy” products. We considered 3 algorithms for this task, including Logistic Regression with the L1 penalty, Random Forest, and XGBoost. All algorithms were tuned using a random grid search with cross-validation on the training set. XGBoost resulted in the highest accuracy of 89% on the training set, and 85% on the test set. We had a similar approach for the regression task, which aimed to directly predict the exact nutrition score of a food product. Again, all three algorithms, which included LASSO, Random Forest, and XGBoost were tuned via random grid search with cross-validation on the training set. XGBoost resulted in the lowest RMSE of 4.13 on the training set and 4.81 on the test set. 
 
