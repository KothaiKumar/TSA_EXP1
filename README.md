## Developed By: Kothai K
## Register Number: 212222240051
##  Date: 
# Ex.No: 01A PLOT A TIME SERIES DATA


# AIM:
To Develop a python program to Plot a time series data for Walmart sales dataset.

# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```python
import pandas as pd
import matplotlib.pyplot as plt
```
```python
file_path = '/content/WMT.csv'  
data = pd.read_csv(file_path)
```
```python
data['Date'] = pd.to_datetime(data['Date'])
```
```python
plt.figure(figsize=(10, 6))
plt.plot(data['Date'], data['Close'], label='Close Price', color='blue')
```
```python
plt.title('WMT Stock Closing Price Over Time')
plt.xlabel('Date')
plt.ylabel('Closing Price')
plt.legend()
plt.grid(True)
```
```python
plt.show()
```

# OUTPUT:

![image](https://github.com/user-attachments/assets/903820d5-c060-4c58-b997-9a1deaece67d)

# RESULT:
Thus, the Python code for plotting the time series of given data is implemented successfully.
