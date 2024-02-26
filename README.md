<img width="427" alt="img3" src="https://github.com/nanditha121/exno1/assets/142209508/86d6e1f8-ff6e-410b-bf85-54a03a4d2b78"># Exno:1
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

# Coding 
           import pandas as pd
df=pd.read_csv("/content/SAMPLEIDS.csv")
df

import pandas as pd
df=pd.read_csv("/content/SAMPLEIDS.csv")
df
df.head()

import pandas as pd
df=pd.read_csv("/content/SAMPLEIDS.csv")
df
df.head()
df.describe()

import pandas as pd
df=pd.read_csv("/content/SAMPLEIDS.csv")
df
df.head()
df.describe()
df.info()

import pandas as pd
df=pd.read_csv("/content/SAMPLEIDS.csv")
df
df.tail()

import pandas as pd
df=pd.read_csv("SAMPLEIDS.csv")
df
df.shape

import pandas as pd
df=pd.read_csv("SAMPLEIDS.csv")
df
df.isnull()

import pandas as pd
df=pd.read_csv("SAMPLEIDS.csv")
df
df.dropna()
#Output:
![ex1](https://github.com/nanditha121/exno1/assets/142209508/31fbd124-d28b-4448-bc44-0d5cc69c9a6a) 

<img width="422" alt="img 2" src="https://github.com/nanditha121/exno1/assets/142209508/09ecb493-5f2e-4c85-b2d0-c5f47b239a12">

<img width="427" alt="img3" src="https://github.com/nanditha121/exno1/assets/142209508/ab49db17-d2d0-41c3-8f1f-bf26fc1e88db">

<img width="375" alt="img4" src="https://github.com/nanditha121/exno1/assets/142209508/71d54184-7e75-4665-9a3e-778b27c89879">

<img width="428" alt="img5" src="https://github.com/nanditha121/exno1/assets/142209508/446ff844-1a6f-4287-aa6d-9fa880df31f6">

<img width="284" alt="img6" src="https://github.com/nanditha121/exno1/assets/142209508/ca6a0857-61c2-49d6-a0b6-422033f57c76">

<img width="386" alt="img7" src="https://github.com/nanditha121/exno1/assets/142209508/767ec547-7224-4582-ba6a-5342af8b194e">

<img width="417" alt="img8" src="https://github.com/nanditha121/exno1/assets/142209508/e555deb7-63bd-4ff0-a7a8-82608c180a15">

# Result
          Thus the given data is read,cleansed and the cleaned data is saved into the file.
