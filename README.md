# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas library and linear_model from sklearn using import statement.

### Step2
Read the given csv file using read_csv().

### Step3
Create two arrays, indenpendent array x withtwo classes and dependent array y with one class. Find the regression of x and y using linear_model. Linear Regression() method and fit x and y using .fit() method.

### Step4
Find the coefficients using coef_and intercept using intercept.

### Step5
Predict the linear regression using regr.predict()method and display the result.

## Program:

Developed by: VAISHNAVI T
Register number: 25017435
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('PredictedCO2 for the corresponding Weight and Volume : ',predictedCO2)
```
## Output:
```
Coefficients: [0.00755095 0.00780526]
Intercept: 79.69471929115939
PredictedCO2 for the corresponding Weight and Volume :  [114.75968007]
```
### Insert your output


<img width="938" height="421" alt="Screenshot 2025-12-24 212446" src="https://github.com/user-attachments/assets/c1b9c756-1174-4dba-bdea-8e54b2b31066" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
