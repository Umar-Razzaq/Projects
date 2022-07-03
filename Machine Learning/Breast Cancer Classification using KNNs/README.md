# Breast Cancer Classification using KNNs

In this notebook I use the Breast Cancer Wisconsin (Diagnostic) Database to create a classifier that can help diagnose patients. For this task I use KNN classifier. The KNN classifier gives **91%** accuracy.

Here the steps we will go through:
- Load the data
- Convert data to dataframe
- Split the DataFrame into `X` (the data) and `y` (the labels).
- Use `train_test_split`, split `X` and `y` into training and test sets `(X_train, X_test, y_train, and y_test)`.
- Use KNeighborsClassifier, fit a k-nearest neighbors (knn) classifier with `X_train`, `y_train` and using one nearest neighbor (`n_neighbors = 1`).
- Using the knn classifier, predict means the class label using the mean value for each feature.
- Using the knn classifier, predict the class labels for the test set `X_test`.
- Find the score (mean accuracy) of the knn classifier using `X_test` and `y_test`.
- 

Here are the things that we will analyse:
- How many features does the breast cancer dataset have?
- What is the class distribution? (i.e. how many instances of `malignant` (encoded 0) and how many `benign` (encoded 1)?)