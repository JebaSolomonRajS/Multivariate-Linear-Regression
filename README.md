# Implementation of Multivariate Linear Regression

## Aim

To write a python program to implement multivariate linear regression and predict the output.

## Equipment’s required:

1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm:

### Step 1:

Import the pandas and scikit-learn libraries.

### Step 2:

Read the data from the csv file.

### Step 3:

Split the data into features (X) and target(y).

### Step 4:

Create and fit the linear linear regression model.

### Step 5:

Print the coefficients and intercepts of the linear regression model.

### Step 6:

Make a prediction.

### Step 7:

Print the predicted CO2 emissions.

### Step 8:

End the Program.

## Program:

```
# Multivariate Linear Regression
# Develpoed by: S.Jeba Solomon Raj
# Register number: 23001618

import pandas as pd
from sklearn import linear_model
import matplotlib.pyplot as plt

f=pd.read_csv("CARS.csv")

X= f[["Weight","Volume"]]
y= f["CO2"]

regr= linear_model.LinearRegression()
regr.fit(X,y)

print("Coefficients:",regr.coef_)
print("Intercept:",regr.intercept_)

predictedCO2= regr.predict([[1200,3200]])
print("Predicted CO2 for the corresponding weight and volume",predictedCO2)

```

## Output:

![output](/out.png)
![output](/cars.png)

## Result

Thus the multivariate linear regression is implemented and predicted the output using python program.
