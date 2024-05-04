# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import Libraries:,Load Data:
2. Encode Categorical Data:Use LabelEncoder to convert the categorical variable 'salary' into numerical format.
3. Define Features and Target:Select the relevant columns as features (X) and the target variable (y).
4. split the data using test_train_split
5. Initialize Model:
6. Make Predictions:
7. Evaluate Model:
8. Predict on New Data:



## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Logesh.N.A
RegisterNumber:  212223240078

import pandas as pd
data=pd.read_csv('Employee.csv')
print(data.head())
print(data.tail())
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
y=data["left"]
y
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
### Data:
![image](https://github.com/Jeshwanthkumarpayyavula/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145742402/fbee3684-7675-41ee-882a-23a35298abe3)
### Encoder:
![image](https://github.com/Jeshwanthkumarpayyavula/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145742402/e5b1cfe0-435a-4a40-b537-f81daf2497dc)
### X-values and y-values
![image](https://github.com/Jeshwanthkumarpayyavula/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145742402/02eb9fc1-8a0f-4e3d-bfea-980444d3e35a)
![image](https://github.com/Jeshwanthkumarpayyavula/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145742402/b7dbbf0a-176b-42f8-9c05-bae5f811696c)
### Accuracy and Prediction
![image](https://github.com/Jeshwanthkumarpayyavula/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145742402/bef4cc93-2dd4-47d8-9d9b-bc8f528e1e71)




## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
