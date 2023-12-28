# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.

### Step2
Read the CSV file.


### Step3
Get the value of X and Y variables.

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 3300kg, and the volume is 1300cm3.

### step6
Print the predicted output.

## Program:
```
import pandas as pd
from sklearn import linear_model
data=pd.read_csv("Cars_multi.csv.csv")
x=data[['Weight','Volume']]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print('predicted CO2 for the corresponding weight and volume',predictCO2)





```
## Output:

![image](https://github.com/Saravanan2512/Multivariate-Linear-Regression/assets/144979117/0eec967f-9c5b-403a-9091-ebc5b69fe13e)

### Insert your output

```
Coefficients: [[0.00755095 0.00780526]]
Intercept: [79.69471929]
predicted CO2 for the corresponding weight and volume [[114.75968007]]
```

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
