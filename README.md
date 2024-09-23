# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
<li> STEP 1: Get the independent variable X and dependent variable Y.</li>
<li> STEP 2: Calculate the mean of the X -values and the mean of the Y -values.</li>
<li> STEP 3: Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png"></li>
<li> STEP 4: Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png"></li>
<li> STEP 5: Use the slope m and the y -intercept to form the equation of the line.</li>
<li> STEP 6: Obtain the straight line equation Y=mX+b and plot the scatterplot.</li>

## Program:
```
import numpy as np
import matplotlib.pyplot as plt

X=np.array(eval(input()))
Y=np.array(eval(input()))
X_mean=np.mean(X)

Y_mean=np.mean(Y)
num=0
denum=0

for i in range(len(X)):
  num+=(X[i]-X_mean)*(Y[i]-Y_mean)
  denum+=(X[i]-X_mean)**2
m=num/denum

for i in range(len(X)):
  num+=(X[i]-X_mean)*(Y[i]-Y_mean)
  denum+=(X[i]-X_mean)**2
m=num/denum
```







## Output:

![Screenshot 2024-08-22 092008](https://github.com/user-attachments/assets/759eff08-6bd7-48ea-b422-3bf7ab081ad0)



## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
