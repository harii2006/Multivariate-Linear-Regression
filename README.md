# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1 Import the required libraries like Pandas and Linear Regression.

### Step2 Create and prepare the dataset with input and output variables.

### Step3 Train the multivariate linear regression model using the dataset.

### Step4 Predict the output using new input values and display the result.

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
predictedCO2 = regr.predict(pd.DataFrame([[3300, 1300]], columns=['Weight', 'Volume']))
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)





```
## Output:


<img width="912" height="93" alt="WhatsApp Image 2026-05-24 at 5 22 20 PM" src="https://github.com/user-attachments/assets/d631593e-d011-4b45-97fa-eb86b9289e47" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
