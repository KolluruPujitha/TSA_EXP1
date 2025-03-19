# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 19-03-2025
### Name:  k.pujitha 

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```p
import pandas as pd
import matplotlib.pyplot as plt

df=pd.read_csv('bank_train.csv')
df.shape

df1=df.head(100)
df1
```
![image](https://github.com/user-attachments/assets/582c0b95-a143-413a-8087-f10dbe939e8d)
```p
df.info()
```
![image](https://github.com/user-attachments/assets/5b07aac1-c506-44bb-b0f8-b7a9893888d9)

```
df.describe
```
![image](https://github.com/user-attachments/assets/e95bd9e6-cba5-499a-b9d4-a13c50fa4b13)

```p
x=df1['age']
y=df1['duration']

plt.figure(figsize=(10,6))
plt.bar(x,y)
plt.grid(True)
plt.title('Duration vs age')
plt.xlabel('age')
plt.ylabel('duration')
plt.show()
```

# OUTPUT:
![image](https://github.com/user-attachments/assets/b5848d73-0a6f-41d1-bbb6-a6ee2c417916)

It is Non-stationary data.

# RESULT:
Thus we have created the python code for plotting the time series of given data.
