# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Normal equation(no iteration)

### Step2
Batch gradient descent

### Step3
Stochastic Gradient Descent

### Step4
Mini-Batch Gradient Descent

### Step5
Gradient Descent with featuring scaling

## Program:
```

import pandas as pd
from sklearn import linear_model
df = pd.read_csv("cars.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)




```
## Output:

<img width="1237" height="354" alt="Screenshot 2026-03-27 002045" src="https://github.com/user-attachments/assets/0908f800-824a-4567-8427-4810b389778a" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
