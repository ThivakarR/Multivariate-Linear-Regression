# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1:

Import panda module as pd
### Step 2:

Import linear model from sklearn
### Step 3:

Read the file cars.csv
### Step 4:

Assign the values for x and y as required
### Step 5:

Create the linearRegression model and predict the output
## Program:
```
'''
Programmed by: R.Thivakar
Register number: 212222240109
'''
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars (1).csv")
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("coefficient",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))
```
## Output:

![Screenshot 2023-06-11 191416](https://github.com/ThivakarR/Multivariate-Linear-Regression/assets/118707074/5b59148f-fae7-4f62-86f0-a45c6d57ebaa)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
