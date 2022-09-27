# Ex03-Univariate-Analysis
## AIM
To perform Univariate EDA on the given data set.

## Explanation
Exploratory data analysis is used to understand the messages within a dataset. This technique involves many iterative processes to ensure that the cleaned data is further sorted to better understand the useful meaning.The primary aim with exploratory analysis is to examine the data for distribution, outliers and anomalies to direct specific testing of your hypothesis.

## ALGORITHM

## STEP 1
Import the built libraries required to perform EDA and outlier removal.

## STEP 2

Read the given csv file

## STEP 3
Convert the file into a dataframe and get information of the data.

## STEP 4
Return the objects containing counts of unique values using (value_counts()).

## STEP 5
Plot the counts in the form of Histogram or Bar Graph.

## STEP 6
Use seaborn the bar graph comparison of data can be viewed.

## STEP 7
Save the final data set into the file

## CODE
/*
~~~
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
df=pd.read_csv("/content/SuperStore.csv")
df.head()
df.info()
df.isnull().sum()
df['Postal Code'] = df["Postal Code"].fillna(df['Postal Code'].mode()[0])
df.isnull().sum()
df.dtypes
df.describe()
sns.boxplot(x='Sales',data=df)
sns.countplot(x='Sales',data=df)
sns.distplot(df["Sales"])
sns.histplot(x='Sales',data=df)
df.skew()
sns.displot(x="Sales",data=df)
df.kurtosis()
plt.figure(figsize=(17,7))
sns.boxplot(x= "Sales" ,data=df)
~~~
*/

## OUTPUT:
![image](https://user-images.githubusercontent.com/103166779/192563643-cc22e666-de3e-4d17-a087-b55405c93d58.png)

![image](https://user-images.githubusercontent.com/103166779/192565359-5f4b6bc7-bcfd-434b-b919-700408cb9578.png)

![image](https://user-images.githubusercontent.com/103166779/192565590-4b7d7c4a-d394-4dbf-b481-4e53c2c7e6c4.png)

![image](https://user-images.githubusercontent.com/103166779/192566052-5555f4b8-4ea9-4f5d-be94-899c183e9de1.png)

![image](https://user-images.githubusercontent.com/103166779/192566786-0967ade6-4290-4b51-8fe8-b7a5d4f80159.png)







