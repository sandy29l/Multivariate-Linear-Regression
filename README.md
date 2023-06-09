## Implementation of Multivariate Linear Regression

# Aim
To write a python program to implement multivariate linear regression and predict the output.

# Equipment’s required:
Hardware – PCs
Anaconda – Python 3.7 Installation / Moodle-Code Runner

# Algorithm:

# Step1
Import panda module as pd

# Step2
Import linear model from sklearn

# Step3
Read the file cars.csv

# Step4
Assign the values for x and y as required

# Step5
Create the linearRegression model and predict the output

# Program:
'''
Developed by: Santhosh L
Register number: 212222100046
'''
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))

# Output:
![maths-10](https://github.com/sandy29l/Multivariate-Linear-Regression/assets/123359969/a4064fea-0994-4c65-a785-b8205765786b)


# Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
