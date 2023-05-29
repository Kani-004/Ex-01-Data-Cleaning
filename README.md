# Ex-01_DS_Data_Cleansing
# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# ALGORITHM
## STEP 1
Read the given Data

## STEP 2
Get the information about the data

## STEP 3
Remove the null values from the data

## STEP 4
Save the Clean data to the file

# CODE
~~~
import pandas as pd df=pd.read_csv("/content/Data_set.csv") print(df) df.head(5) df.info() df.isnull().sum() df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0]) df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0]) df['original_network']=df['original_network'].fillna(df['aired_on'].mode()[0]) df.head() df['rating']=df['rating'].fillna(df['rating'].mean()) df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean()) df.head() df['watchers']=df['watchers'].fillna(df['watchers'].median()) df.head() df.info() df.isnull().sum()
~~~
# OUPUT

![image](https://github.com/Kani-004/Ex-01-Data-Cleaning/assets/129577149/1c514870-8645-424d-8cb4-95c0145a61cb)

# df.head()

![image](https://github.com/Kani-004/Ex-01-Data-Cleaning/assets/129577149/36c672fe-5baa-4093-bbb1-d8a8f3f0607d)

# df.info()

![image](https://github.com/Kani-004/Ex-01-Data-Cleaning/assets/129577149/5db7350a-5578-4cc0-a506-a26d820e47a3)

# df.isnull().sum()

![image](https://github.com/Kani-004/Ex-01-Data-Cleaning/assets/129577149/08effc8a-d92d-49fb-a5f6-d42c321c7433)

# Result:
~~~
Hence the given data is read and perform data cleaning and save the cleaned data to a file.
~~~


