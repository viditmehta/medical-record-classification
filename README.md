# Medical Record Classification

In this study, the goal is to predict patients that will not show up for medical appointments based on their medical records. I use the Kaggle dataset from https://www.kaggle.com/joniarroba/noshowappointments for this project. Briefly, I do the following:

1. Data cleanup. (cleaning column names, remove negative ages etc.)
2. Creation of test and training sets.
3. Creation of a preprocessing pipeline using scikit to prepare the data for the ML algorithms. I standardized the numerical variables, and transformed categorical variables into one or more numerical values. I also performed logarithmic transformation to age data to make it less skewed.

Next I used a variety of classification methods like Decision Tree, a Random Forest, a linear SVM and an SVM with a radial basis kernel to fit the transformed data. I started with default parameters and then used 10-fold cross validation to estimate performance of each of the above methods using both accuracy and AUC as metrics. I also trained an AdaBoost and xgBoost classifiers, and performed ensemble learning on the dataset. 
