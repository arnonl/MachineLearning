**This repository contains a code file that can analyze the data collected during the study “Predicting Barbell Lift Performance with Accelerometer Data”**

Here are the steps taken to analyze this study:

- Download the necessary files from the project website.

- Load the training and final testing data, and perform elementary data analysis.

- Preprocess the data, and omit the redundant features. For this purpose, select the columns which have most of the entry are NA and blank, and filter out the training and test data set and build the validate data set that use to train the model.At this phase, perform the elementary data analysis on newly build training data set.

- Dividing the data into training and testing sets with cross-validation using the “caret” package.

- Now find out the less useful or useless predictor from the training data set, and update the training data set.

- Fit a model on the training data set i.e apply “train()” function where method is random forest algorithm (mehtod = “rf”). In order to speed up the execution trControl parameter of the “train” function is used.

- Fit an alternative model on the training data set using the decision tree algorithm.

- Print the fitted model (the better one) and check out the accuracy of the model.

- Predict the classe of each instance of the reshaped test data set by using “prediction” function of the caret package.

- Estimates out of sample error appropriately with cross-validation