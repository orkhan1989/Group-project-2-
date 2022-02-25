# Group-project-2-

# Introduction:
The goal of our project was to see if key company financial ratios could be used to predict whether future stock returns would increase or decrease. We used  Logistic Regression and Random Forest  machine learning models along with the model enhancing technique Gradient Boosting.
Data:
 We used data from SimFin and opted for the paid SimFin+ version of the database since this greatly expanded the amount of data available for download. As a side note, SimFin uses only organically grown data, sourced from local data farmers!

# Data Preparation:
Working with API pull from SimFin+ we accessed financial ratios and stock prices starting January 2007.
We remove companies that were not currently trading.
We dropped the following columns:
Open; Low; High; Close; Dividend; Volume; Shares Outstanding; SimFinId.  “df_ratios”
We created a daily return column by using the pct_change function on the “Adj Close” column with a
 -1 shift =” prices_df”
We then combined the ratio_df with the prices_df using the defined function “combiner” and the merge function. 
We then segmented the company tickers into the binary categories “0” for percent change less than zero and “1” for percentage change greater than one.
We used the counter function to see if there is a class imbalance.
We applied Standard Scaler on X_train and X_test



Models:
The four steps applied to each of our machine learning models are:
1.	Preprocess the data
2.	Train the data (being careful to only use the training data)
3.	Validate the model (using the test data that was partitioned prior to training the model)
4.	Make Predictions with the predict function of the model.

Random Forest:
For our first model we chose Random Forest, an ensemble learning method under the supervised learning category. The model works by generation many binary decision trees and the choosing the output as the class selected by the most trees.
Random Forest Algorithm offers several advantages:
•	It’s robust against overfitting
•	It can handle a very large number of input variables
•	It’s robust to outliers
•	More robust against noise
•	It’s robust to non-linear data
•	It tends to run efficiently with very large data sets.

Logistic Regression:
Logistic Regression is also a supervised machine learning model, which uses the logistic function to model a binary dependent variable, hence, positive or negative; true or false; fraud not fraud and so on. The Logistic Function can take any real number and map it to a number between zero and one. In essence Logistic Regression predicts the probability that an instance belongs to a particular class and if the probability is greater than 50% then the instance is said to belong to that class.


Gradient Boosting:
Most generally Boosting is a technique to convert “weak learners” to “strong learners” Boosting Algorithms  work iteratively, by sampling more heavily the observations with worst predictions. Subsequent weak learners then aggregated to produce a more accurate and precise prediction. The goal of a boosting algorithm is to combine weak learners into ensemble learners. Boosting algorithms are considered meta-algorithms, which, instead of working with and affecting data, boosting algorithms work with other algorithms.

Model Evaluation Metrics
Confusion Matrix:

The F1 calculation:
F1 = 2x(precision x recall) / (precision + recall) = TP / (TP + ½(FP + FN))
F1 = 1 for a model with perfect precision and recall


