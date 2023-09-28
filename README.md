# Loan-Eligiblity-Prediction-Project

Created this Data Science project in Python using a few libraries such as: Pandas, Numpy, Matplotlib, Sklearn.
The dataset used in this analysis is taken from Kaggle website
For first dataset called train the link is: https://www.kaggle.com/datasets/ninzaami/loan-predication     
For second dataset called test the link is: https://www.kaggle.com/datasets/vikasukani/loan-eligible-dataset

# The method used in this analysis are: 
1. Decision Tree Classification method
2. Naive Bayes Classification method

# To perform the analysis I've used Jupyter Notebook.
First I've imported the "train" dataset into the notebook and Checked the data, after checking I found who was eligible for loan and who wasn't. 
Then I used the boxplot graph to check for the Applicant Income, to clarify if they can Repay the loan if provided.
Then Ploted Histogram to identify the co-realtion of Applicant Income and Coapplicant Income.
After that I used Boxplot to Cross check the relation of Applicant Income with Education.
Then I used another Boxplot, Histogram method to check for Loan Amount.
I created a new Column called "LoanAmount_log" to check the Count of the Applicants.
After cleaning the data created another Column called "TotalIncome" by adding Applicant Income with Coapplicant Income, then created another Column called "TotalIncome_log" to check the Count of total Applicants. 

# Performed Data Cleaning:
Using '.isnull( ).sum( )' function calculated the total number of null values in the Dataset.
Using '.mode( )[0], .mean( )' function filled the missing values.

# Decision Tree Classification method:
Using ".iloc[:,np.r_[columns tags].values" function collected the values of that columns in a variable, then converted those values using "LabelEncoder" from "sklearn" library into binary code for the Machine learning algorithm to run it faster.
Using "DecisionTreeClassifier", "metrics" from "sklearn" library calculated the accuracy of the Loan Prediction.

# Naive Bayes Classification method:
Using "GaussianNB" from "sklearn" libray calculated the accuracy of the Loan Prediction.

# Conclusion:
Calculating from both method the better accuracy was given from the "Naive Bayes method".

# Calculations on Test Data:
Used all the above method mentioned above to calculate the accuracy on the test data. The method used in this dataset is "Naive Bayes Method" because the accuracy of that method was quite better then the "Decision Tree method".
