# Exno:1 Data Cleaning Process

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

# Coding and Output:
```
import pandas as pd
import numpy as np
import seaborn as sns
import os 
df=pd.read_csv("SAMPLEIDS.csv")
df
```
![o1](https://github.com/nanditha121/exno1/assets/142209508/ad624ae6-bfed-444c-97b5-a894757560c9)

```
import pandas as pd
df=pd.read_csv("/content/SAMPLEIDS.csv")
df
df.head()
```

```
import pandas as pd
df=pd.read_csv("/content/SAMPLEIDS.csv")
df
df.head()
df.describe()
```

```
import pandas as pd
df=pd.read_csv("/content/SAMPLEIDS.csv")
df
df.head()
df.describe()
df.info()
```

```
import pandas as pd
df=pd.read_csv("/content/SAMPLEIDS.csv")
df
df.tail()
```

```
import pandas as pd
df=pd.read_csv("SAMPLEIDS.csv")
df
df.shape
```

```
import pandas as pd
df=pd.read_csv("SAMPLEIDS.csv")
df
df.isnull()
```

```
import pandas as pd
df=pd.read_csv("SAMPLEIDS.csv")
df
df.dropna()
```



![ex1](https://github.com/nanditha121/exno1/assets/142209508/31fbd124-d28b-4448-bc44-0d5cc69c9a6a) 

![ex1](https://github.com/nanditha121/exno1/assets/142209508/3e139bd7-c428-4522-a468-2f5e4f97e747)

![ex1](https://github.com/nanditha121/exno1/assets/142209508/09ecb493-5f2e-4c85-b2d0-c5f47b239a12)

![ex1](https://github.com/nanditha121/exno1/assets/142209508/ab49db17-d2d0-41c3-8f1f-bf26fc1e88db)

![ex1](https://github.com/nanditha121/exno1/assets/142209508/71d54184-7e75-4665-9a3e-778b27c89879)

![ex1](https://github.com/nanditha121/exno1/assets/142209508/446ff844-1a6f-4287-aa6d-9fa880df31f6)

![ex1](https://github.com/nanditha121/exno1/assets/142209508/ca6a0857-61c2-49d6-a0b6-422033f57c76)

![ex1](https://github.com/nanditha121/exno1/assets/142209508/767ec547-7224-4582-ba6a-5342af8b194e)

![ex1](https://github.com/nanditha121/exno1/assets/142209508/e555deb7-63bd-4ff0-a7a8-82608c180a15)

# Result
Thus the given data is read,cleansed and the cleaned data is saved into the file.
