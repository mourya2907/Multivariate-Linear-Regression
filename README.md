# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>Collect and preprocess the data

### Step2
<br>Formulate the multivariate linear regression model. The equation for multivariate linear regression.

### Step3
<br>Define the cost function to be minimized. The most common function used for linear regression is the Mean Square Error(MSE)

### Step4
<br>Use an optimization algorithm to minimize the cost function. The most common optimization algorithm used for linear regression.

### Step5
<br>Evaluate the performance of the model using metrics.

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car.csv")
df.info()
df.head()
df.tail()
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)






```
## Output:
![alt text](<Screenshot 2025-01-01 204739.png>)



<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
