# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.Get the independent variable X and dependent variable Y.


2.Calculate the mean of the X -values and the mean of the Y -values.


3.Find the slope m of the line of best fit using the formula.

![image](https://github.com/Dineshsekhar2004/Univariate-Linear-Regression/assets/119405916/19ce192f-4a21-4b7f-8402-8fe298ce6c8f)

4.Compute the y -intercept of the line by using the formula:

![image](https://github.com/Dineshsekhar2004/Univariate-Linear-Regression/assets/119405916/4abb11ba-0f54-4653-8c46-4fd62cd565e5)

5.Use the slope m and the y -intercept to form the equation of the line.


6.Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```

Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Dinesh.S
Register number: 212222230033
import numpy as np
import matplotlib.pyplot as plt
x=np.array(eval(input()))
y=np.array(eval(input()))
xmean=np.mean(x)
ymean=np.mean(y)
num,den=0,0
for i in range(len(x)):
  num+=(x[i]-xmean)*(y[i]-ymean)
  den+=(x[i]-xmean)**2
m=num/den
c=ymean-m*xmean
print(m,c)
y_pred=m*x+c
print(y_pred)
plt.scatter(x,y)
plt.plot(x,y_pred,color="orange")
plt.show()

```
## Output
![image](https://github.com/Dineshsekhar2004/Univariate-Linear-Regression/assets/119405916/701dbcc8-192a-4b3f-a6d7-6733188c7682)


## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
