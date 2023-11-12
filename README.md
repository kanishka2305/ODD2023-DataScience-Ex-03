# ODD2023-DataScience-Ex-03
# Aim:
To read the given data and perform the univariate analysis with different types of plots.

Explanation: Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.
# Alogorithm:
Step1: Read the given data.

Step2: Get the information about the data.

Step3: Remove the null values from the data.

Step4 :Mention the datatypes from the data.

Step5 :Count the values from the data.
# Program:
```py
Developed By : Kanishka.V.S
Register number: 212222230061

# Superstore.csv:
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv('SuperStore.csv')
print(df)
df.head()
df.info()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
df.describe()

### Diabetes.csv:
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
df.kurtosis()

### employeesal.csv:

import pandas as pd
df=pd.read_csv("/content/employeesal.csv")
df
df.info()
df.dtypes
df['Salary'].value_counts()
df.describe()
import seaborn as sns
sns.boxplot(x='Experience_Years',data=df)
sns.countplot(x="Experience_Years",data=df)
sns.distplot(df['Experience_Years'])
sns.histplot(x="Experience_Years",data=df)
df.skew()
sns.histplot(x='Salary',data=df)
sns.distplot(df['ID'])
df.kurtosis()
sns.boxplot(x='Salary',data=df)
sns.boxplot(x='Experience_Years',data=df)
```
# Output:
# Superstore.csv:
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/18699d91-13c8-42da-a30a-8a7a30295a8a)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/a755e6f6-715f-422f-a701-353ff67bee98)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/d4cbb2bb-13a0-40a8-8e8e-e1e71c754de7)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/6005f380-0056-44de-9d01-bb76942d2688)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/d088dc80-6eae-4d86-90b5-d6cf94c6bb4c)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/5dada865-e66b-4fbd-a25c-f453f3f4f16a)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/3c5725b7-16fc-4e83-b737-a343cb968de4)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/2911d05a-2994-4ea4-978b-670dcbfebfe3)
# Diabetes.csv:
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/d70cf471-5f5e-45fa-a534-09fa43b2208d)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/4f8f922b-fcc3-46c9-9640-bdc4889d0f10)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/1f79f55a-e689-43b4-8bd1-bf0aec62bfd3)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/a6e2ce67-7fc1-4627-8e40-0cf5f415e811)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/1da0654f-aa7d-40b1-ad50-0d542c34f67e)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/b291156c-5c8e-4f34-a6f1-0998cb872849)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/973d8dc9-97a1-44bc-9149-ffbaa8b5f12d)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/3ac60bab-9063-48c2-aedc-048b9db6aab6)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/2aa8b784-69e3-4e02-aee3-8d82b80f9293)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/a9246dc1-49fe-44b4-8d2c-fddbc7d8d7c0)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/cfce8782-fdcd-423c-a9c6-ec9fa9b8fa97)
# employeesal.csv:
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/2613e7c1-ca9e-4835-ad86-6d7e343d1a29)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/d36be6d3-b06e-4ab8-8e0d-d238da6e97c0)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/4e837ce6-d663-4fd4-a408-b9b1c4d6017f)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/f0ac4405-467c-4620-b5c3-dff03d46f4cc)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/33d03c17-0124-4c97-a5c9-4a7b417f0d54)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/f57af9f6-649f-4d8e-8bdd-06db645e5662)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/29b72786-d590-423f-8fef-e778203dfabe)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/ebd864ce-6054-44fd-900c-1f89ef3831b2)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/d18b39a5-ebd8-4b46-a874-33b1cb011e71)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/466ff74a-f928-402b-8cba-b7f004fb37a6)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/4fd4ada4-1941-41d9-9fab-d3369944be04)
![image](https://github.com/kanishka2305/ODD2023-DataScience-Ex-03/assets/113497357/18340295-e039-48c4-a812-2d0246758240)
# Result:
Hence the univariate analysis is verified
