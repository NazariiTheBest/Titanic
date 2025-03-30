# Titanic
Survivality prediction of the Titanic passengers

Firstly, we need to import required libraries. 
Set the <b>matplotlib inline</b> for rendering directly in the notebook. And then importing required libraries.

Secondly, import data from the csv file named titanic. Also check the imported dataset

![image](https://github.com/user-attachments/assets/a640853e-635e-4d98-beee-d4f1cefdfc2c)


Thirdly, check dtypes of the DataFrame columns, check the info about DataFrame. As we can see, it contains <b>891</b> rows and <b>12</b> columns.
As we can see, we have the missing values in the DataFrame. What 

![image](https://github.com/user-attachments/assets/28cb6380-c4a7-4335-afa4-4f80cce8a540)

We can make conclusion, that columns PassengerId and Name has no sense for Machine Learning model. So we'll use DataFrame withoud these columns.
Also column named Cabin has a lot of missing values, so we'll drop it.

![image](https://github.com/user-attachments/assets/576b6c76-9cde-43a6-8211-2ae7fd4ea613)


Then we need to split DataFrame into training and testing in the next way: 80% for train, 20% for test
The next step is to train LogisticRegression model from <b>Scikit-learn</b>

Evaluating model with cross validation:

![image](https://github.com/user-attachments/assets/91a8a396-be3b-4405-b4d1-0a014cf24953)

Plot the confusion matrix:

![image](https://github.com/user-attachments/assets/7642e29c-f804-4ffb-bbdf-491a8c23372a)

Printing Classification Model Metrics: Precision, Recall, Sensitivity, Specifity

![image](https://github.com/user-attachments/assets/0fffcd5e-435e-4755-9913-27e686107f37)

Now I'm interested to check if male and female with same conditions survive (Female, 42y.o., 1 class and Male, 42y.o, 1 class):

![image](https://github.com/user-attachments/assets/27fe9db8-e940-4888-9fa3-80acdba1a598)


