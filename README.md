# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas and import linear_model from sklearn.
### Step2
Read the csv file using pd.read_csv() function.
### Step3
Find the regression using linear_model.LinearRegression().
### Step4
Find the regression coefficient and  regression intercept.
### Step5
Predict the output.
## Program:
```
Developed by : JANANI.S
RegisterNumber:22008491
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[1995,522]])
print("Predicted CO2 emissiom based on weight and volume:",predictedCO2)
```
## Output
![multivariate](https://user-images.githubusercontent.com/119477549/214572585-1cce3b91-7569-4c20-9b5f-461bd806ea71.png)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
