# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required libraries.

2.Upload and read the dataset.

3.Check for any null values using the isnull() function.

4.From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.

5.Find the accuracy of the model and predict the required values by importing the required module from sklearn.
## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: YUVARAJ JOSHITHA
RegisterNumber:212223240189
import pandas as pd
data=pd.read_csv("dataset/Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evalution","number_project","average_montly_hours","time_spend_company","work_accident","promotion_last_5years","salary"]]
x.head()
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])  
*/
```

## Output:
# Data Head:
![image](https://github.com/Joshitha-YUVARAJ/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145742770/26197dba-361d-420f-a3fa-d4f21eb87d2f)

# Data set info:
![image](https://github.com/Joshitha-YUVARAJ/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145742770/ceb3c545-c9c7-4822-a9ad-008ab3a60e71)

# Null dataset:
![image](https://github.com/Joshitha-YUVARAJ/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145742770/86e61b4d-1e9b-43f5-9b25-d5ac18de2997)
# Values count in left column:
![image](https://github.com/Joshitha-YUVARAJ/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145742770/516fe028-3802-4b66-970a-46a8f698b074)

# Dataset transformed head:
![image](https://github.com/Joshitha-YUVARAJ/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145742770/6aece108-e9e6-452a-aebe-852e4647e034)

# x.head:
![image](https://github.com/Joshitha-YUVARAJ/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145742770/573294e2-2f6d-4a33-9d6e-ab87a7193e2e)
# Accuracy:
![image](https://github.com/Joshitha-YUVARAJ/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145742770/45890b8e-334c-48ba-aac4-e2353651a353)
# Data Prediction:
![image](https://github.com/Joshitha-YUVARAJ/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145742770/e3c818d8-b901-453c-9e5d-f9ecb18a6a9a)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
