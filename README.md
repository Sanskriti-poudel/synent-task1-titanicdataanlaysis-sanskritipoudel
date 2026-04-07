Titanic Dataset – Data Cleaning & Preprocessing
Problem Statement
The goal of this task is to clean and preprocess the Titanic dataset so that it becomes suitable for further analysis or building machine learning models. The dataset contains missing values, inconsistent data types, and unnecessary columns, which need to be handled properly.

Dataset Details
The dataset used is the Titanic dataset, which contains information about passengers such as:
Passenger ID
Name
Age
Gender
Ticket class
Fare
Cabin
Embarked location
Survival status

Approach
1. Loading and Exploring Data
Imported required libraries like pandas and numpy
Loaded dataset using read_csv()
Checked shape, data types, and summary statistics
Performed basic EDA using info() and describe()
2. Handling Missing Values
Checked null values using isnull()
Filled missing values in Embarked column using mode
Dropped Cabin column because it had too many missing values
Filled missing Age values using average age based on passenger titles (Mr, Miss, etc.)
3. Feature Engineering
Extracted Title from the Name column
Used title to group passengers and estimate missing age values
4. Removing Duplicates
Checked duplicate rows using duplicated()
No major duplicates found
5. Data Type Conversion
Converted:
Survival column → category
Age → integer
Fare → integer
6. Renaming Columns
Renamed columns to make them more readable:
PassengerId → ID
Survived → Survival_Status
Pclass → Ticket_Class
Name → Passenger_Name
Sex → Gender
Results

After preprocessing:
All missing values were handled properly
Unnecessary column (Cabin) was removed
Data types were corrected
Column names were made clearer
Dataset is now clean and ready for analysis or modeling
