# ANALYSIS OF ENGLISH PREMIER LEAGUE USING MACHINE LEARNING ALGORITHMS
In this paper we make multiple classifiers to predict the outcomes of English Premier League matches.
## Abstract
This paper aims to predict the outcome of a given match in the English Premier League (EPL) using multiple classification algorithms and analyze and report the differences between the performance of the classifiers. There are 20 CSV files with the rows being a particular match, one for each year of the EPL from 2000-2019. For each match, we have a few characteristics about the match, some of them are: which team was the home team, what was the number of shots by each team, what was the number of shots on target, what were the betting statistics of the match, and many more.We also have the final standings of the 43 teams in each year consolidated into a single file, each row represents a team and each attribute is the year of the standing. Using the given data, in this paper, we will apply feature engineering after cleaning and preprocessing the data, and implement the following classifiers: KNN, Logistic Regression, Bayes Classifier, SVM, and a Neural Network, and then finally report on the differences in performance of each classifier. We concluded that our classifiers perform best with feature normalisation and using PCA to reduce the dimensionality of data. All classifiers except logistic regression were giving us an accuracy of about 60% and the reason why logistic regression may not be performing as well was due to outliers in the data.

## Classification Algorithms Used in the Model:
- Naïve Bayes Classifier (Generative classifier)
- Neural Networks
- K-Nearest Neighbors (Instance-based classifier)
- SVM
- Logistic Regression (Discriminative classifier)

## Performance Evaluation Metrics
- Model’s Accuracy
- Model’s Sensitivity/Recall
- Model’s Specificity/Precision
- The F1 Score

## Data Preprocessing
- Data Cleaning
- Data Splitting and Transformation
- Data Reduction

## Feature Engineering
- Feature Extraction And Data Preparation
- Scaling and PCA

## Implementation
- Models Without Scaling and PCA
- Models With Scaling and PCA
- Models Lower Training Set (80-20 split)
- Models Balanced Classes

## Performance Evaluation
- With Preprocessing
- Without Preprocessing
- Lesser Training Data
- Balanced Classes

## Conclusion
In conclusion, we started off with raw data of each season of the EPL. From this raw data, we extracted useful features that would tell us about the history of each team. We then used feature scaling and PCA to reduce the dimensionality of the data, which gave us the best accuracies (around 60%). We also found out that due to class imbalance, our models were having a hard time predicting the draw result, and when we balanced the
classes, it performed better for the draw class, but worsened on the other classes. We also concluded that a higher amount of training data was improving our results. Thus we believe, having more data would have improved our models significantly. Other than having less data to train on, we were also unable to extract other key features from the raw data that might have an impact on the outcome of a game. Some of them include factors such as the player lineups of the team and player injuries. Including such features would also help our models perform better.