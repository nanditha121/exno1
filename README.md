# Exno:1
Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output
```
import pandas as pd
df=pd.read_csv("/content/SAMPLEIDS.csv")
df
```
![image](https://github.com/nanditha121/exno1/assets/142209508/d0b3136a-8be2-463c-a806-555e77ba084b)

```
print(df.head(7))
```
![image](https://github.com/nanditha121/exno1/assets/142209508/68ac5355-f2da-4c1b-86a7-eb2262cf53c5)

```
print(df.tail(2))
```
![image](https://github.com/nanditha121/exno1/assets/142209508/1bb41619-3058-47c3-84ae-33e65e105a50)

```
df.info()
```
![image](https://github.com/nanditha121/exno1/assets/142209508/06ee54a4-5f69-4688-9d74-57f26a4e9f06)

```
print(df.describe())
```
![image](https://github.com/nanditha121/exno1/assets/142209508/ebe720de-b53c-4b3c-a58d-2f6a743df293)

```
df.isnull().sum()
```
![image](https://github.com/nanditha121/exno1/assets/142209508/75842dfc-1ce9-401c-a40a-243506dc99b4)
'''
df.nunique()
```
![image](https://github.com/nanditha121/exno1/assets/142209508/727504a4-1d40-41f9-ac8d-dcba517764cd)
```
mn=df.TOTAL.mean()
mn
```
![image](https://github.com/nanditha121/exno1/assets/142209508/8f9618cb-4975-4e66-b66f-81aeb5bf821a)

```
df.TOTAL.fillna(mn,inplace=True)
df
```
![image](https://github.com/nanditha121/exno1/assets/142209508/ea68d87c-70e5-4911-a0cb-29638f339ca3)
```
min=df.M4.min()
min
```
![image](https://github.com/nanditha121/exno1/assets/142209508/888406a9-b30c-47b3-9ae4-5247ab6c3d6c)

```
df.M4.fillna(min,inplace=True)
df
```
![image](https://github.com/nanditha121/exno1/assets/142209508/e5a10ca8-aeea-4844-8dee-78bc1fd64951)


![image](https://github.com/nanditha121/exno1/assets/142209508/24f2bb99-116f-4d42-bc58-32681041e196)

```
import pandas as pd
import seaborn as sns
age=[1,3,28,27,25,92,30,39,40,50,26,24,29,94]
af=pd.DataFrame(age)
af
```
![op1](https://github.com/nanditha121/exno1/assets/142209508/6f32e692-6fe2-4232-81e7-28d1fb5c91eb)

```
sns.boxplot(data=af)
```
![op2](https://github.com/nanditha121/exno1/assets/142209508/8abcba48-4605-49fb-9853-426b1cfa177e)

```
sns.scatterplot(data=af)
```
![op3](https://github.com/nanditha121/exno1/assets/142209508/a2be70ad-b285-43ce-a99f-b96533035c59)

```
q1=af.quantile(0.25)
q2=af.quantile(0.50)
q3=af.quantile(0.75)
iqr=q3-q1
iqr
low=q1-1.5*iqr
low
high=q3+1.5*iqr
high
```
![op4](https://github.com/nanditha121/exno1/assets/142209508/f0c25649-ec32-410f-ae59-4972a3aa3290)
```
af=af[((af>=low)&(af<=high))]
af
```
![op5](https://github.com/nanditha121/exno1/assets/142209508/87b861b8-c373-432f-bad2-347e117c759a)
```
af.dropna()
```
![op6](https://github.com/nanditha121/exno1/assets/142209508/256be38d-c6d1-4b50-b96c-01b67444c1a2)
```
sns.boxplot(data=af)
```
![op7](https://github.com/nanditha121/exno1/assets/142209508/a4ce213a-1cc7-4e6a-9888-eef1381cb3d4)

```
sns.scatterplot(data=af)
```
![op8](https://github.com/nanditha121/exno1/assets/142209508/bf9b871f-35e7-4075-940a-ff9eb295fbfa)

```
data=[1,12,15,18,21,24,27,30,33,36,39,42,45,48,51,54,57,60,63,66,69,72,75,78,81,84,87,90,93,96,99,102,105]
df=pd.DataFrame(data)
df
```
![op9](https://github.com/nanditha121/exno1/assets/142209508/52ac6a7f-0988-405d-88df-617669e5463c)
```
import numpy as np
from scipy import stats
z=np.abs(stats.zscore(df))
z
```
![op10](https://github.com/nanditha121/exno1/assets/142209508/d9b9181b-fce3-4fb2-8a42-71214cea2dd3)

# Result
Thus the given program executed successfully.
