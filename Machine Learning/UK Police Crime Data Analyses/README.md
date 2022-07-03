# UK Police Crime Data Analyses

In this report, we aim to answer the following questions using Machine Learning and Data Mining:
- Are violent crimes in UK increasing with time?
- Where is the highest per head crime rate in UK?

## Pre-processing and EDA
To answer the above questions we perform pre-processing and EDA using Pandas. 

1. The claim seems to be true. Even though the data suggests that crimes follow a cyclical pattern in which crime tends to be high in the months of June, July and august, a simple glance at the peaks of these cycles suggests that every consecutive year the number of crimes tend to be higher. Additionally, the troughs of each cycle seem to be increasing with time proving that violent crime also increases with time. Irrespective of the monthly fluctuations, there seems to be a general year on year increase in the trend of crime rates. This can be seen in the figure 1.1, given below:
![crime-rate](./crime%20rate%20and%20time.png)

2. Eyeballing the histograms (figure 1.2) plotted below, it is easily understood that crime rate in Birmingham stands at around 60459, which is way higher than any of the other locations. Only Manchester and Leeds come close to competing with the number of crimes in Birmingham, but they still fall short.
The red line in the following graphs show the frequency of crimes in Birmingham:
![crime-type](./crime%20type%20and%20location.png)


## Prediction, Clustering and Outlier Analyses
### Perform cluster analyses on the data, primarily on location and crime types:
For cluster analyses, we used K-modes algorithm for clustering based on location and crime types. Both variables being categorical, made K-modes a very viable choice for clustering here. To determine the optimal value of K, we first randomly sampled 10,000 rows and ran the clustering for different values of K, and then plotted the graph. After which elbow method was used. We did this three times to ensure convergence to the real value of K. This gave out 2 as the optimal value of K.

###  Given a crime predict its outcome:
For predicting the outcome of a crime. We used the variables listed below, which are a mix of numeric and categorical type.
1. crime_type (Categorical) Values: 0-5
2. Variable: Males; measures: Value (Numeric)
3. Variable: Females; measures: Value (Numeric)
4. Variable: Lives in a household; measures: Value (Numeric)
5. Variable: Lives in a communal establishment; measures: Value (Numeric)
6. Variable: Schoolchild or full-time student aged 4 and over at their non-term-time address; measures:
Value (Numeric)
7. Variable: Density (number of persons per hectare); measures: Value (Numeric)
8. Region (Categorical)
After which we first converted the numerical variables into categorical using binning techniques. Due to computing power constraint, we selected 3 bins for each numerical variable. Then, using a train – test split of 20%, we trained a decision tree classifier based on entropy. Like the ID3 algorithm it chooses roots recursively based on the variable which has the least Entropy. This classifier would classify an outcome given the above variables. Outcome variable had missing values which were filled by “No information” as the missing values itself had meaning. To justify this, we can think of a crime type whose outcome usually is ambiguous and then it is given a missing value. The model had an accuracy of 73% and can output the outcome of a given crime.

### Interesting findings:
- Cyclic nature of the crimes: As shown in the figure above in claim 1, crimes follow a cyclic pattern in
UK. According to the data, there is an increase in the number of crimes in the summers of 2015, 2016, 2017 and 2018. On the other hand, the number of crimes decrease during winters.
- Relationship between crime and population: It can be seen from the four graphs in part two that the following areas have the highest crime rates in UK: Birmingham, Manchester, Leeds, Bradford and Liverpool. These areas with crime rate happen to be the most populated areas in the UK. This shows that population and crime rate are highly correlated in UK.