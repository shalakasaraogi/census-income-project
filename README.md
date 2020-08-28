# US-Census-Income-Project  

## Description  

In this project, initially we preprocess the data and then develop an understanding of different features of the data by performing exploratory analysis and creating visualizations. Further,after having sufficient knowledge about the attributes, performed a predictive task of classification to predict whether an individual makes over 50K a year or less,by using different Machine Learning Algorithms.  

## Dataset   

The "Census Income" dataset from the UCI Machine Learning Repository that contains the income information for over 48,000 individuals taken from the 1994 US census.  

For more details about this dataset, you can refer to the following link: https://archive.ics.uci.edu/ml/datasets/census+income  


![census-income](https://user-images.githubusercontent.com/62024191/91567404-b0c52b80-e962-11ea-86d7-18476314e5e7.png)  


## Lab Environment  

RStudio  

## Domain  

Social  

## Tasks Done  

**1. Data Preprocessing:**  

a)	Replaced all the missing values with NA.  
b)	Removed all the rows that contain NA values.    
c)	Removed all whitespaces from the columns.  

**2. Data Manipulation:**  

Performed data manipulation to analyze the data set using various functions from the dplyr package.  

a)	Extracted the “education” column and stored it in “census_ed” .  
b)	Extracted all the columns from “age” to “relationship” and stored it in “census_seq”.  
c)	Extracted the column number “5”, “8”, “11” and stored it in “census_col”.  
d)	Extracted all the male employees who work in state-gov and stored it in “male_gov”.  
e)	Extracted all the 39 year olds who either have a bachelor's degree or who are native of United States and stored the result in “census_us”.  
f)	Extracted 200 random rows from the “census” data frame and stored it in “census_200”.  
g)	Get the count of different levels of the “workclass” column.  
h)	Calculated the mean of “capital.gain” column grouped according to “workclass”.  

**3. Data Visualization:**  

a)	Built a bar-plot for the “relationship” column and filled the bars according to the “race” column.   
b)	Built a Histogram for the “age” column with number of bins equal to 50.  
c)	Built a scatter-plot between “capital.gain” and “hours.per.week”. Map “capital.gain” on the x- axis and “hours.per.week” on the y-axis.  
d)	Built a box-plot between “education” and “age” column.Map “education” on the x-axis and “age” on the y-axis.  

**4. Linear Regression:**  

a)	Built a simple linear regression model as follows:  

i)	Divided the dataset into training and test sets in 70:30 ratio.  
ii)	Built a linear model on the test set where the dependent variable is “hours.per.week” and independent variable is “education.num”.  
iii)	Predicted the values on the train set and found the error in prediction.  
iv) Calculated the root-mean-square error (RMSE).  

**5. Logistic Regression:**  

a)	Built a simple logistic regression model as follows:  

i)	Divided the dataset into training and test sets in 65:35 ratio.  
ii)	Built a logistic regression model where the dependent variable is “X”(yearly income) and independent variable is “occupation”.  
iii)	Predicted the values on the test set.  
iv)	Ploted accuracy vs cut-off and picked an ideal value for cut-off.  
v)	Built a confusion matrix and calculated the accuracy.  
vi)	Ploted the ROC curve and found the auc(Area Under Curve).   

b) Built a multiple logistic regression model as follows:  

i)	Divided the dataset into training and test sets in 80:20 ratio.  
ii)	Built a logistic regression model where the dependent variable is “X”(yearly income) and independent variables are “age”, “workclass”, and “education”.  
iii)	Predicted the values on the test set.  
iv)	Ploted accuracy vs cut-off and picked an ideal value for cut-off.
v) Built a confusion matrix and calculated the accuracy.  
vi) Ploted the ROC curve and calculated the auc(Area Under Curve).  

**6. Decision Tree:**  

a)	Built a decision tree model as follows:  

i)	Divided the dataset into training and test sets in 70:30 ratio.  
ii)	Built a decision tree model where the dependent variable is “X”(Yearly Income) and the rest of the variables as independent variables.  
iii) Ploted the decision tree.  
iv)	Predicted the values on the test set.  
v)	Built a confusion matrix and calculated the accuracy.  

**7. Random Forest:**  

a)	Built a random forest model as follows:  

i)	Divided the dataset into training and test sets in 80:20 ratio.  
ii)	Built a random forest model where the dependent variable is “X”(Yearly Income) and the rest of the variables as independent variables and number of trees as 300.  
iii)	Predicted values on the test set  
iv)	Built a confusion matrix and calculated the accuracy  
