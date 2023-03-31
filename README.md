# Ex03-Univariate-Analysis

## Aim:
To read the given data and perform the univariate analysis with different types of plots.

## Explanation:

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## Algorithm:

### Step1:

Read the given data.

### Step2:

Get the information about the data.

### Step3:

Remove the null values from the data.

### Step4:

Mention the datatypes from the data.

### Step5:

Count the values from the data.

### .Step6:

Do plots like boxplots,countplot,distribution plot,histogram plot.

## Program:

DEVELOPED BY : MATHAVAN S

REGISTER NO : 212221220031

import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv('superstore.csv')
df

df.head()
df.info()
df.describe()
df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x='Postal Code',data=df)

### Output:

### Dataset:
![image](https://user-images.githubusercontent.com/129484178/229034954-8db6673b-2d8b-480f-9d92-e8ef9e06d1f1.png)

### Head:
![image](https://user-images.githubusercontent.com/129484178/229035099-bb31ed8d-0d68-40a4-b109-ef5a55fff3c5.png)

### Info:
![image](https://user-images.githubusercontent.com/129484178/229035220-a20fff42-ce44-49ca-8665-9fdc1a0aa0c0.png)
### Describe:
![image](https://user-images.githubusercontent.com/129484178/229035349-49e1d612-3b58-4747-b5fe-b8b9b109e76b.png)

### Isnull:
![image](https://user-images.githubusercontent.com/129484178/229035411-1424dcf6-842d-44cd-a2c3-c27b68cd5f26.png)

### dtypes:
![image](https://user-images.githubusercontent.com/129484178/229035460-609af648-01eb-4547-a14e-283c3b21509c.png)

### Valuecount:
![image](https://user-images.githubusercontent.com/129484178/229035531-9881749a-fef2-41ef-8b1d-014ab6260794.png)

### Boxplot:
![image](https://user-images.githubusercontent.com/129484178/229035602-051aec4c-4e1c-4158-b647-dbb8a172f0d4.png)

### Countplot:
![image](https://user-images.githubusercontent.com/129484178/229035708-b71cba61-da29-4a6c-92db-069e6c782fea.png)

### Distribution plot:
![image](https://user-images.githubusercontent.com/129484178/229035801-1dc04161-3a88-4535-87f3-19f6b3025069.png)

### Histogram plot:
![image](https://user-images.githubusercontent.com/129484178/229035893-65014ba7-ca6e-419a-baff-cfbd8851c5b9.png)

### Result:

Thus we have read the given data and performed the univariate analysis with different types of plots.
