#### DEVELOPED BY : PRAVEEN S
#### REG NO : 212222240078
####  Date: 
# Ex.No: 01A PLOT A TIME SERIES DATA

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
```py
import pandas as pd
import matplotlib.pyplot as plt
import numpy as n
```
```py
data = pd.read_csv('/content/OnionTimeSeries - Sheet1.csv')
```
```py
data['Date'] = pd.to_datetime(data['Date'])
```
```py
plt.figure(figsize=(12, 6))
plt.plot(data['Date'], data['Min'], label='Minimum cost')
plt.xlabel('Date')
plt.ylabel('Min')
plt.title('Cost Of Onion')
plt.grid(True)
plt.show()
```






# OUTPUT:
![image](https://github.com/user-attachments/assets/d8d305f7-b2aa-4515-bace-c6a9dcc55ee2)






# RESULT:
Thus we have created the python code for plotting the time series of given data.
