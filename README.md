# EX 10: Implementation of Multivariate Linear Regression
## Date: 08.11.23
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1:

Import panda

### Step2:

Import linear model from sklearn

### Step3:

Read the file cars.csv

### Step4:

Assign the values for x and y as required

### Step5:

Create the linearRegression model and predict the output

## Program:
```
#To write a python program to implement multivariate linear regression and predict the output.
# Program Developed By: DIVYA.A
# Register Number : 212222230034
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("/content/cars (1).csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCo2=regr.predict([[300,1300]])
print("Predicted CO@ for the corresponding weight and volume",predictedCo2)
```
## Output:

![math exp 10](https://github.com/Divya110205/Multivariate-Linear-Regression/assets/119404855/6f2cd7f3-24e7-4c50-82fd-f1206a97a465)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
