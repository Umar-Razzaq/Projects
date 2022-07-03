# Supervised Learning

We'll explore the relationship between model complexity and generalization performance, by adjusting key parameters of various supervised learning models. Part 1 of this notebook will look at regression and Part 2 will look at classification.

## Part 1 - Regression
 A function that fits a polynomial LinearRegression model on the *training data* `X_train` for degrees 1, 3, 6, and 9. (Use PolynomialFeatures in sklearn.preprocessing to create the polynomial features and then fit a linear regression model) For each model, find 100 predicted values over the interval x = 0 to 10 (e.g. `np.linspace(0,10,100)`) and store this in a numpy array. The first row of this array should correspond to the output from the model trained on degree 1, the second row degree 3, the third row degree 6, and the fourth row degree 9.
- Polynomial Features in LinearRegression model
- Fit Polynomial Features in LinearRegression model
- Model fit (Underfitting, Overfitting, Good_Generalization)
- Regularizaiton

## Part 2 - Classification
Here's an application of machine learning that could save your life! For this section we will be working with the [UCI Mushroom Data Set](http://archive.ics.uci.edu/ml/datasets/Mushroom?ref=datanews.io) stored in `mushrooms.csv`. The data will be used to train a model to predict whether or not a mushroom is poisonous.
- Get important features
- Support Vector Classifier
- Model fit (Underfitting, Overfitting, Good_Generalization)