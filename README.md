# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
## REGISTER NUMBER : 212224230273
## COMPLETED BY : Srimeganathan S



import numpy as np
X= np.array(eval(input()))
Y= np.array(eval(input()))
X_mean=np.mean(X)
Y_mean=np.mean(Y)
num=0
denom=0
for i in range(len(X)):
  num+=(X[i]-X_mean)*(Y[i]-Y_mean)
  denom=(X[i]-X_mean)**2
  m=num/denom
  c=Y_mean-m*X_mean
  print(m,c)
  Y_pred=m*X+c
  print(Y_pred)

  import matplotlib.pyplot as plt
  plt.scatter(X,Y,color='RED')
  plt.plot(X,Y_pred,color='blue')
  plt.show()
```



## Output
<img width="1077" height="738" alt="image" src="https://github.com/user-attachments/assets/69bc1076-0ff7-4e8f-a68f-4573fc5b2a38" />
<img width="769" height="613" alt="Screenshot 2025-10-17 101911" src="https://github.com/user-attachments/assets/5979f026-be53-4008-b4b0-c9b17717555c" />
<img width="777" height="567" alt="Screenshot 2025-10-17 101925" src="https://github.com/user-attachments/assets/03ce859a-75ed-4a41-88ef-f69c5162d8ab" />
<img width="878" height="573" alt="Screenshot 2025-10-17 101934" src="https://github.com/user-attachments/assets/b4f8de81-4bdd-45c4-835d-95aded11fb7c" />
<img width="831" height="569" alt="Screenshot 2025-10-17 101945" src="https://github.com/user-attachments/assets/3c6869be-7663-441a-a2e9-05f65d046441" />
<img width="820" height="563" alt="Screenshot 2025-10-17 101953" src="https://github.com/user-attachments/assets/4fd73cea-3951-4177-a9d3-82ae90e919db" />


## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
