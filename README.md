# Exno:1
Data Cleaning Process

## AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

## Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

## Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

## Coding and Output:
```
# Developed By: LAAKSHIT D
# Register Number: 212222230071
```
#### 1) Read CSV file
```
import pandas as pd
df=pd.read_csv('/content/SAMPLEIDS.csv')
df
```
<img height=50% width=50% src="https://github.com/laakshit-D/exno1/assets/119559976/a210fb07-bd74-49a3-ae3a-32ef13bf8eb7">

#### 2) DISPLAY THE INFORMATION ABOUT CSV AND RUN THE BASIC DATA ANALYSIS FUNCTIONS
```
df.info()
df.describe()
```
![image](https://github.com/laakshit-D/exno1/assets/119559976/eb36dbf7-bf22-4b71-be77-91cbd617bd7e) <img height=70% width=50% src="https://github.com/laakshit-D/exno1/assets/119559976/b5a9a89e-823b-4f14-9787-b0bfef4291f6">

#### 3) CHECK OUT NULL VALUES IN DATA SET
```
df.isnull().sum()
```
![image](https://github.com/laakshit-D/exno1/assets/119559976/4818844c-c7d6-4151-ad4f-11da73020930)

#### 4) DISPLAY THE SUM ON NULL VALUES IN EACH ROWS
```
df.isnull().sum(axis=1)
```
![image](https://github.com/laakshit-D/exno1/assets/119559976/04ba9496-d19f-437f-a73e-be600337cd3b)

#### 5) Drop the null values
```
df.dropna(inplace=True)
df
```
<img height=70% width=70% src="https://github.com/laakshit-D/exno1/assets/119559976/cca1df8d-5392-45c0-8589-9b3136fcf6fd">
>


# Result
          <<include your Result here>>
