# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>Import the pandas library using the statement import pandas as pd.

### Step2
<br>Import the linear_model module from scikit-learn using the statement from sklearn import linear_model.

### Step3
<br>Read the CSV file named "cars.csv" using the pd.read_csv() function and store the data in a DataFrame named df.

### Step4
<br>Get the value of X and y variables and Create the linear regression model and fit.

### Step5
<br>Predict the CO2 emission using the trained linear regression model by calling the predict() method on regr [[3300, 1300]]

### Step6
<br>Print the Predicted CO2

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("/content/cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO@ for the corressponding weight and volume",predictedCO2)

```
## Output:
![Screenshot 2023-06-03 153519](https://github.com/Adhithyaram29D/Multivariate-Linear-Regression/assets/119393540/b21037cf-2d25-44be-9bc1-d12776f4485e)


<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
