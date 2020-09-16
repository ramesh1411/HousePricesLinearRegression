# HousePricesLinearRegression
Predicting house prices using Linear Regression and Gradient Boosting Regressor

I am going to work on a dataset which consists information about the location of the house , price and other aspects such as square feet etc. When working on these sort of data , we need to see which column is important for us and which is not. The aim is to make a model which can give us a good prediction on the price of the house based on other variables. I am going to use Linear Regression for this dataset and see if it gives us a good accuracy or not. I am aiming to achieve an accuracy score of 85%+
Below steps were followed to develop the model:
1. We import our libraries and dataset and then we see the head of the data to know how the data looks like and use describe function to see the percentile’s and other key       statistics.
2. We will do data visualization and also going to see how and what can we infer from visualization. The plot that we used is scatter plot , scatter plot helps us to see how our data points are scattered and are usually used for two variables. I did some data cleaning and pre-processing
3. We import our dependencies , for linear regression we use sklearn (built in python library) and import linear regression from it.
4. We then initialize Linear Regression to a variable reg.
5. Now we know that prices are to be predicted , hence we set labels (output) as price columns and we also convert dates to 1’s and 0’s so that it doesn’t influence our data much. We use 0 for houses which are new that is built after 2014.
6. We again import another dependency to split our data into train and test.
7. I’ve made my train data as 90% and 10% of the data to be my test data , and randomized the splitting of data by using random_state.
8. I train data , test data and labels for both aand fit our train and test data into linear regression model.
9. After fitting our data to the model we can check the score of our data ie , prediction. in this case the prediction is 73%
10. As we didn't get the desired accurecy, I am going to use Gradient Decent Boosting 
11. We first import the library from sklearn 
12. We create a variable where we define our gradient boosting regressor and set parameters to it , here
n_estimator — The number of boosting stages to perform. We should not set it too high which would overfit our model.
max_depth — The depth of the tree node.
learning_rate — Rate of learning the data.
loss — loss function to be optimized. ‘ls’ refers to least squares regression
minimum sample split — Number of sample to be split for learning the data
13. We then fit our training data into the gradient boosting model and check for accuracy
14. We got an accuracy of 91.94% 

Note: I will be uploading a new project for the same problem statement and solve it without using Gradient Decent Boosting

