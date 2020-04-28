# Predict wages by years of experience (Simple Linear Regression)
Predicting wages by years of experience in a small enterprise. In this case it was applied simple linear regression because there is just one independent variable.


# SIMPLE LINEAR REGRESSION:

## 1) Importing libraries:
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
import statistics as sta

## 2) Importing the dataset
dataset = pd.read_csv('wages.csv')
X = dataset.iloc[:, :-1].values
y = dataset.iloc[:, 1].values


print("Mean of wages =", y.mean())
print("Median of wages =", np.median(y))
print("Standard Deviation (STD) =", round(sta.stdev(y),2))
print("Variance =", round(sta.variance(y),2))
