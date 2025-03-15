# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 15-03-2025

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
```
import pandas as pd
import matplotlib.pyplot as plt

# Load the CSV file
file_path = "weather_classification_data.csv"  # Replace with your actual file path
data = pd.read_csv(file_path)

# Generate a date index assuming daily records
data.index = pd.date_range(start="2025-01-01", periods=len(data), freq="D")

# Plot the time series of 'Temperature'
plt.figure(figsize=(10, 6))
plt.plot(data.index, data["Temperature"], label="Temperature", color="red")

# Customize the plot
plt.title("Temperature Over Time")
plt.xlabel("Date")
plt.ylabel("Temperature (°C)")
plt.grid(True)
plt.legend()

# Display the plot
plt.show()
```









# OUTPUT:![image](https://github.com/user-attachments/assets/7840be99-af0d-4121-bca2-774041daae15)








# RESULT:
Thus we have created the python code for plotting the time series of given data.
