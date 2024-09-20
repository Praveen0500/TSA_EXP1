#### DEVELOPED BY : PRAVEEN S
#### REG NO : 212222240078
####  Date: 
# Ex.No: 01A PLOT A TIME SERIES DATA

# AIM:
To Develop a python program to Plot a time series data (Price of the Onion).
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

plt.plot(data['Date'].head(100), data['Min'].head(100), label='Minimum cost')

plt.xlabel('Date')
plt.ylabel('Min')
plt.title('Cost of Onion (First 100 Data Points)')
plt.grid(True)
plt.legend()
plt.xticks(rotation=45)  
plt.tight_layout()  
plt.show()

```






# OUTPUT:
![Untitled](https://github.com/user-attachments/assets/55d80c35-a9f6-479b-86d9-e6af799f60a0)






# RESULT:
Thus we have created the python code for plotting the time series of given data.
