# Linear Classification
There are two pieces of codes in this zip file: hepatitis and bankruptcy, which are composed of the two datasets given in the first mini-project. Please upload the two datasets in the form of .csv file to the folder named “content” after you open the codes in Google Colab. The execution of the codes will need the datasets. Please click “Runtime”, and then “Run all” to execute all codes.

For each dataset, there are three sections: data analysis, initial logistic regression models with basic features, and cross-validation with feature selection.
Data analysis: the datasets are read and segregated using pandas. Then, numerical features are normalized. After, the histograms of many variables are plotted to show the distributions.
Logistic regression: the initial classification models are built with the basic features and the performance is evaluated in this section. In the classes called “hep_model” and “bank_model”, the “fit” module finds the best weight for each feature using gradient descent. There are learning rates and three types of stopping criteria to be defined by the users when calling this module. Then, the “predict” module returns the predictions using the weights obtained. Afterwards, a function called “Accu_eval” evaluates the predictive accuracy. Afterwards, the impact of learning rate and stopping criterion on performance is studied and the results are recorded in the tables.

K fold cross-validation is used in 4 parts of the project,
1, to check the stability of the best model we found, run the validation 10 times 
the following 3 part is the process of finding the best model
2, to compare the model with different subsets of features, which were selected by feature selection based on the Maximal Information Coefficient (MIC).
3, to compare the model with different subsets of features, which were selected by removing features with low variance.
4, to compare the model with a different order, which was get by using the Polynomial Curve Fitting method after feature selection


