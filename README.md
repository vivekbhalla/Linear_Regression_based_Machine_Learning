Linear Regression Based Machine Learning
========================================

This project is to implement regression on web search ranking dataset.

Total number of features in the dataset is 46.
The dataset contains the relevance of some web pages labeled by humans for a set of queries. The relevance values are 0, 1 and 2, where higher value indicates higher relevance. The dataset contains 15211 Samples or Rows which are divided into 40%, 10% and 50% for the training phase, validation phase and the testing phase respectively. 

The train phase calculates the trained weights (train.m). These weights are used by the validation phase to predict the target values and looking at the root mean square error of the validation phase the parameters in the train phase are adjusted to get best results i.e. least error. Finally after the best result is obtained these weights are used to predict target values for test data and the final error in the test data is calculated and reported.
 
Two regression models were used. The first regression model was Linear Regression using Gaussian Basis Functions (predict.m). The second regression model was the Nonlinear Neural Network Model with Levenberg-Marquardt backpropagation training function (nn_model.m). The best performance for the Linear Regression Model using Gaussian basis function was observed by setting the Model Complexity M at 3 and the Regularization Parameter Lambda at 100. The final Root Mean Square Error for the test data was observed to be 0.518812

Note: All the data has already been loaded in the ‘project1_data.mat’ file.
