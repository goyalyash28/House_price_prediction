# House_price_prediction
This contains code of machine learning of House price prediction

LINEAR REGRESSION:-
First we did this project by linear regression. Regression works on the line equation , y=mx+c , trend line is set through the data points to predict the outcome.
The variable we are predicting is called the criterion variable and is referred to as Y. The variable we are basing our predictions on is called the predictor variable and is referred to as X. When there is only one predictor variable, the prediction method is called Simple Regression. and if multiple predictor variable are present then multiple regression.

We import our dependencies , for linear regression we use sklearn (built in python library) and import linear regression from it.
We then initialize Linear Regression to a variable reg.
Now we know that prices are to be predicted , hence we set labels (output) as price columns and we also convert dates to 1’s and 0’s so that it doesn’t influence our data much . We use 0 for houses which are new that is built after 2014.
We again import another dependency to split our data into train and test.
I’ve made my train data as 90% and 10% of the data to be my test data , and randomized the splitting of data by using random_state.
So now , we have train data , test data and labels for both let us fit our train and test data into linear regression model.
After fitting our data to the model we can check the score of our data ie , prediction. in this case the prediction is 73%

The accuracy of the model is lower than our aim of 85. So how do we achieve that 85% target ?


GRADIENT BOOSTING:-
For building a prediction model , many experts use gradient boosting regression , so what is gradient boosting ? It is a machine learning technique for regression and classification problems, which produces a prediction model in the form of an ensemble of weak prediction models, typically decision trees.


We first import the library from sklearn ( trust me , it is the best library for all statistical related models)
We create a variable where we define our gradient boosting regressor and set parameters to it , here
n_estimator — The number of boosting stages to perform. We should not set it too high which would overfit our model.
max_depth — The depth of the tree node.
learning_rate — Rate of learning the data.
loss — loss function to be optimized. ‘ls’ refers to least squares regression
minimum sample split — Number of sample to be split for learning the data
3. We then fit our training data into the gradient boosting model and check for accuracy
4. We got an accuracy of 91.94% which is good
