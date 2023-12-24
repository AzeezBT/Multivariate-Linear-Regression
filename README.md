# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>

### Step2
<br>

### Step3
<br>

### Step4
<br>

### Step5
<br>

## Program:
```
#To write a python program to implement multivariate linear regression and predict the output.
#Developed by: Azeez Ahamad
#Ref.No: 23003977

import pandas as pd
from sklearn import linear_model
import matplotlib.pyplot as plt

df=pd.read_csv("cars.csv")

x=df[['Weight', 'Volume']]
y=df['CO2']

regr=linear_model.LinearRegression()
regr.fit(x,y)

#coefficients and intercept of model
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)

predictedCO2= regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)
```
## Output:
![image](https://github.com/AzeezBT/Multivariate-Linear-Regression/assets/150319523/2f41d3a0-1a9c-476e-9df6-73b6df6441dc)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
