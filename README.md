# Implementation of Multivariate Linear Regression
## Date:18.05.2024
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import Pandas library.

### Step2
Import Linear_model from sklearn.

### Step3
Read the csv file using pandas library.

### Step4
Enter the parameters of the linear function.

### Step5
Print the parameters of the linear function. End the program.

## Program:
```

Developed by: kavipriya sp
Reg.No: 2305002011
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
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
![WhatsApp Image 2024-05-28 at 10 39 11 AM](https://github.com/kavipriyasp07/Multivariate-Linear-Regression/assets/155508590/ef72e26c-12c8-4887-8859-9542cf92b4ad)

### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
