# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import and Load Data

### Step2
Select Input and Output

### Step3
Train the Model

### Step4
Display Results & Predict

## Program:
```python
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)






```
## Output:


<img width="918" height="279" alt="Screenshot 2026-03-17 185218" src="https://github.com/user-attachments/assets/6ea525f4-4043-4153-b50f-2594b5f97f1c" />

<img width="701" height="79" alt="Screenshot 2026-03-17 185228" src="https://github.com/user-attachments/assets/c845f4f9-13a4-4153-b3eb-2823b9acd8a7" />


### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
