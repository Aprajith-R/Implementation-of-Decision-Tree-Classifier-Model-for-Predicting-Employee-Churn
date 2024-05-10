# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the required libraries.
2. Upload and read the dataset.
3. Check for any null values using the isnull() function.
4. From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.
5. Find the accuracy of the model and predict the required values by importing the required module from sklearn.  

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Aprajith R
RegisterNumber: 212222080006
import pandas as pd
data=pd.read_csv("Employee.csv")
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
![Screenshot 2024-05-10 220843](https://github.com/Aprajith-R/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/161153978/e5408d83-d766-427c-881e-6d63bf992e23)

![Screenshot 2024-05-10 220853](https://github.com/Aprajith-R/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/161153978/641e6562-dc7f-456a-b612-7ace91ca3ac9)

![Screenshot 2024-05-10 220904](https://github.com/Aprajith-R/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/161153978/574028d4-32e3-4193-8616-f90ca306ba3e)

![Screenshot 2024-05-10 220913](https://github.com/Aprajith-R/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/161153978/672723ae-5d79-4390-9f1f-4627ed87f4d0)

![Screenshot 2024-05-10 220921](https://github.com/Aprajith-R/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/161153978/2eb26cc7-0cf8-4947-96d4-ce253c56aceb)

![Screenshot 2024-05-10 221022](https://github.com/Aprajith-R/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/161153978/cb8b681f-361f-4c1e-b020-0f73475bec7e)

![Screenshot 2024-05-10 221033](https://github.com/Aprajith-R/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/161153978/aedc37fd-a14a-4577-a37f-59a6de255659)

![Screenshot 2024-05-10 221045](https://github.com/Aprajith-R/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/161153978/de4b7f4f-a8ad-4464-a5e2-d71fa813078c)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
