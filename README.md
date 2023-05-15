# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the standard libraries.
2. Upload the dataset and check for any null values using .isnull() function.
3. Import LabelEncoder and encode the dataset.
4. Import DecisionTreeRegressor from sklearn and apply the model on the dataset.
5. Predict the values of arrays.
6. Import metrics from sklearn and calculate the MSE and R2 of the model on the dataset.
7. Predict the values of array.
8. Apply to new unknown values

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: Pooja A
RegisterNumber: 212222240072
import pandas as pd
data=pd.read_csv("Salary.csv")
data.head()

data.info()

data.isnull().sum()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()

data["Position"]=le.fit_transform(data["Position"])
data.head()

x=data[["Position","Level"]]
x.head()

y=data[["Salary"]]

from sklearn.model_selection import train_test_split
x_train, x_test, y_train, y_test=train_test_split(x,y,test_size=0.2,random_state=2)

from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)

from sklearn import metrics
mse=metrics.mean_squared_error(y_test, y_pred)
mse

r2=metrics.r2_score(y_test,y_pred)
r2

dt.predict([[5,6]])
*/
```

## Output:
### initial dataset:
![238249522-3013f142-8d1c-42cc-9f11-751ce674ae84](https://github.com/poojaanbu0/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119390329/770f2fce-5e51-477f-bf37-64b5bf435379)

### Data Info:
![238249556-f42b2f9a-d161-4205-90ca-368733c1c156](https://github.com/poojaanbu0/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119390329/b1ef72ac-5b61-4986-95e2-248a4329623f)

### Optimization of null values:
![238249588-d0eefc95-353f-4c35-b696-de3a978d8124](https://github.com/poojaanbu0/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119390329/8fbad043-0c47-4b03-8f35-14f57fa3955f)

### Converting string literals to numerical values using label encoder:
![238249653-4d7e562c-9a2a-48ca-ae0e-5b5f1a429e91](https://github.com/poojaanbu0/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119390329/83e60ae8-f7c4-4e40-82ae-6b69ac7a9e25)

### Assigning x and y values:
![238249701-c56e3af8-065e-45de-93a5-ce9910f6638d](https://github.com/poojaanbu0/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119390329/5402f71c-0a39-4e17-a446-1da090502489)

### Mean Squared Error:
![238249743-29e082dc-8dc0-4836-ba51-334497170c7a](https://github.com/poojaanbu0/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119390329/c3583929-9130-46f1-a36f-c0bef5d1f00d)

### R2 (variance):
![238249774-0fe196e4-baea-44e6-8a90-240185d0cbe7](https://github.com/poojaanbu0/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119390329/d06edfb3-dcc3-45c4-841e-a43845e26937)

### Prediction:
![238249776-e69d2f5c-67f7-462a-9ddc-20a51c383016](https://github.com/poojaanbu0/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119390329/24921d06-acc8-4587-80a3-fc271762f0bf)

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
