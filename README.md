# Feature_Importance
This Python script performs logistic regression and feature importance analysis on a dataset called 'no_show.csv'. Here's a description of the script:

The required libraries are imported: numpy, matplotlib.pyplot, pandas, and seaborn.
The dataset is loaded using pd.read_csv() into a pandas DataFrame called df.
The features of interest are specified in the features list.
Categorical features ('Gender' and 'Neighbourhood') are encoded as dummy variables using mapping and factorization techniques.
The sigmoid function is defined, which calculates the sigmoid of a given input.
The logistic regression function is defined, which performs logistic regression using gradient descent to optimize the weights.
The feature matrix X is extracted from the DataFrame, and the target variable y is created by converting 'No-show' values to binary labels.
The logistic regression model is trained by calling the logistic_regression() function with the specified number of iterations and learning rate.
Predictions are made by applying the sigmoid function to the dot product of the feature matrix and the learned weights.
The accuracy of the model is evaluated by comparing the predictions with the true labels.
The feature importance is calculated by taking the absolute values of the learned weights.
A pandas DataFrame called feature_importance is created, which contains the features and their corresponding importance scores.
The feature_importance DataFrame is sorted in descending order by importance.
A bar plot is created using seaborn.barplot() to visualize the feature importance.
The plot is labeled and titled, and then displayed using matplotlib.pyplot.show().

This script can be used to analyze the importance of different features in predicting the likelihood of a no-show appointment based on the provided dataset.
