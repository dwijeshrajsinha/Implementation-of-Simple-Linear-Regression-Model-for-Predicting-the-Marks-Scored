# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import necessary libraries (e.g., pandas, numpy,matplotlib)
2. Load the dataset and then split the dataset into training and testing sets using sklearn library. 
3. Create a Linear Regression model and train the model using the training data (study hours as input, marks scored as output). 
4. Use the trained model to predict marks based on study hours in the test dataset. 
5. Plot the regression line on a scatter plot to visualize the relationship between study hours and marks scored.

## Program:
```
import numpy as np
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression

x = np.array([1,2,3,4,5]).reshape(-1,1)
y = np.array([40,50,60,70,80])

model = LinearRegression()
model.fit(x,y)

slope = model.coef_[0]
intercept = model.intercept_
print(slope)
print(intercept)

plt.scatter(x,y,color="blue")
plt.plot(x,model.predict(x),color="red")
plt.xlabel("hours studied")
plt.ylabel("marks obtained")
plt.title("Linear regression")
plt.legend("")
plt.grid(color="yellow")
plt.show()
```
```
Developed by: DWIJESH RAJ SINHA Y
RegisterNumber: 25013468
```

## Output:
<img width="1314" height="626" alt="image" src="https://github.com/user-attachments/assets/5b7e2c90-3f2c-4166-9416-a0c65186ad1b" />
<img width="863" height="667" alt="image" src="https://github.com/user-attachments/assets/135c4404-7ba5-4756-9e9e-aa1d95f8c751" />


## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
