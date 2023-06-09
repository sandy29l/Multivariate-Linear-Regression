# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1:
import pandas as pd

### Step2:
Read the csv file

### Step3:
Get the values of x and y variables.

### Step4:
Create the linear regression model and fit.

### Step5:
Predict the CO2 emission of a car where the weight is 3300kg, and the vlume is 1300cm3.

### Steop6:
Print the predicted output.

## Program:
```
'''
Developed by: Vanitha S
Register number: 212222100057
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

```
## Output:
![maths-10](https://github.com/sandy29l/Multivariate-Linear-Regression/assets/123359969/4999bb2b-13fc-4bd7-aefc-801e7b3f5694)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
