# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: V RISHON ANAND
RegisterNumber:  24900460
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from sklearn.metrics import mean_absolute_error,mean_squared_error
df=pd.read_csv('student_scores.csv')
print(df)
df.head(0)
df.tail(0)
print(df.head())
print(df.tail())
x = df.iloc[:,:-1].values
print(x)
y = df.iloc[:,1].values
print(y)
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=1/3,random_stat
from sklearn.linear_model import LinearRegression
regressor = LinearRegression()
regressor.fit(x_train,y_train)
y_pred = regressor.predict(x_test)
print(y_pred)
print(y_test)
# graph plot for training data
plt.scatter(x_train,y_train,color='black')
plt.plot(x_train,regressor.predict(x_train),color='blue')
plt.title("hours vs Scores(training set)")
plt.xlabel("hours")
plt.ylabel("Scores")
plt.show()
# graph plot for test data
plt.scatter(x_test,y_test,color='black')
plt.plot(x_train,regressor.predict(x_train),color='red')
plt.title("hours vs Scores(testing set)")
plt.xlabel("hours")
plt.ylabel("Scores")
plt.show()
mse=mean_absolute_error(y_test,y_pred)
print('MSE = ',mse)
mae=mean_absolute_error(y_test,y_pred)
print('MAE = ',mae)
rmse=np.sqrt(mse)
print("RMSE= ",rmse)
*/
```

## Output:
![simple linear regression model for predicting the marks scored](sam.png)
![Screenshot 2024-10-17 095111](https://github.com/user-attachments/assets/9abd028b-f568-4e53-82f1-5e6ab297b2fe)
![Screenshot 2024-10-17 095252](https://github.com/user-attachments/assets/6ddc0883-6e6c-43f2-8e01-eb3cb3d2737d)
![Screenshot 2024-10-17 095347](https://github.com/user-attachments/assets/0daaf3bb-e5fb-4357-9583-8ae9e689c599)
![Screenshot 2024-10-17 095440](https://github.com/user-attachments/assets/eca12131-9e9f-47fd-88bb-4ccbbd9e7f47)
![Screenshot 2024-10-17 095513](https://github.com/user-attachments/assets/b9a32432-6433-4a1b-9302-19d07281e61a)


## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
