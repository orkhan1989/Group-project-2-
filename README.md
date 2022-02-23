# Group-project-2-

Data from SimFin

Introduction:

In this project out goal was to use two of the machine learning models that we covered in class, Logistic Regression and Random Forest.
to classify our data set of financial ratios and returns. 
The four steps applied to each of our machine learning models are:
1.	Preprocess the data
2.	Train the data(being careful to only use the training data)
3.	Validate the model (using the test data that was partitioned prior to training the model)
4.	Make Predictions with the predict function of the model.


Models
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
The Logistic Function is defined as follows:
1/(1+e-t)
