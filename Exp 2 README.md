# Experiment 2: Data Visualization Using Matplotlib and Seaborn

## Aim

To visualize data using Matplotlib and Seaborn libraries.

## Algorithm

1.  **Start.**
2.  Import the Matplotlib and Seaborn libraries.
3.  Load data into a Pandas DataFrame.
4.  Plot a histogram for age distribution using `plt.hist()`.
5.  Plot a scatter plot for Age vs. Salary using `sns.scatterplot()`.
6.  Plot salary distribution using `sns.boxplot()`.
7.  Show the plots sequentially.
8.  **Stop.**


## Program
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

data = pd.DataFrame({
    'Age': [22, 25, 28, 30, 35, 40, 45, 50],
    'Salary': [20000, 25000, 30000, 35000, 40000, 50000, 60000, 70000]
})

plt.hist(data['Age'], bins=5, edgecolor='black')
plt.title("Age Distribution")
plt.xlabel("Age")
plt.ylabel("Frequency")
plt.show()

sns.scatterplot(x='Age', y='Salary', data=data)
plt.title("Age vs Salary")
plt.show()

sns.boxplot(y=data['Salary'])
plt.title("Salary Distribution")
plt.show()

## output
<img width="725" height="577" alt="image" src="https://github.com/user-attachments/assets/1b5d1a66-bd9f-4b9c-81af-ec276d441630" />
<img width="721" height="507" alt="image" src="https://github.com/user-attachments/assets/bbe855ef-a6dc-4194-a649-098da6b5fcd1" />



## result


