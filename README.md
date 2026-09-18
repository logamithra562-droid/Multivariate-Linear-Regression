# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Load the required libraries and prepare the dataset.

### Step2
Separate the input variables (X) and output variable (Y).

### Step3
Split the dataset into training and testing data.

### Step4
Train the multivariate linear regression model using the training data.

### Step5
Predict the output using the trained model and evaluate the result.

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regression = linear_model.LinearRegression()
regression.fit(X, y)
print(regression.coef_)
print(regression.intercept_)
print("Predicted value:",regression.predict([[3300,1300]]))





```
## Output:
![alt text](<Screenshot 2026-09-03 122731.png>)
### Insert your output



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.