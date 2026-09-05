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
import numpy as np
import matplotlib.pyplot as plt

X = np.array(eval(input()))
Y = np.array(eval(input()))

Xmean = np.mean(X)
Ymean = np.mean(Y)
num,den = 0,0
for i in range(len(X)):
    num += (X[i]-Xmean)*(Y[i]-Ymean)
    den += (X[i]-Xmean)**2
slope = num/den
c = Ymean-slope*Xmean
    
print (slope, c)

Y_pred = slope*X + c
print (Y_pred)

plt.scatter(X,Y)
plt.plot(X,Y_pred,color="pink")
plt.show()






```
## Output:
![alt text](<Screenshot 2026-09-05 090056.png>)
### Insert your output



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.