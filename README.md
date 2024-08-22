# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

### STEP1: 
Get the independent variable X and dependent variable Y.
### STEP2:
Calculate the mean of the X -values and the mean of the Y -values.
### STEP3: 
Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
### STEP4: 
Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
### STEP5: 
Use the slope m and the y -intercept to form the equation of the line.
### STEP6: 
Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: RIYA P L
RegisterNumber: 212223240141
import numpy as np
import matplotlib.pyplot as plt

# Preprocessing input data
X = np.array(eval(input()))
Y = np.array(eval(input()))

# Mean
X_mean =np.mean(X)
Y_mean =np.mean(Y)
num=0 #for slope
denom=0 #for slope

#to find sum of (xi-x') & (yi-y') & (xi-x'0)^2
for i in range(len(X)):
    num+=(X[i] -X_mean)*(Y[i]-Y_mean)
    denom+= (X[i]-X_mean)**2

#calculate slope
m=num/denom

#calculate intercept
b=Y_mean-m*X_mean
print(m,b)

#Line equation
y_predicted=m*X+b
print(y_predicted)

#to plot graph
plt.scatter(X,Y)
plt.plot(X,y_predicted,color='red')
plt.show()
*/
```

## Output:
![Screenshot 2024-08-22 091304](https://github.com/user-attachments/assets/b8d43e0b-988e-4bae-9bdf-75b0135bfe79)
![Screenshot 2024-08-22 091314](https://github.com/user-attachments/assets/7fc63de3-bda0-4f7d-afcc-55906ba378f6)
![Screenshot 2024-08-22 091324](https://github.com/user-attachments/assets/9377793f-2859-4d52-beb9-06297e7f1d63)

## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
