# Data_cleaning
🧹 Data Cleaning - Marketing Campaign Dataset
🔧 What I Did
Loaded the dataset using pandas.read_csv() with sep="\t" (tab-separated file).

Removed rows with missing values, especially in the Income column.

Dropped duplicate rows to avoid repetition.
Converted Dt_Customer to proper datetime format.

Created new columns:

Total_Spent: Sum of all amount spent columns.

TotalAcceptedCmp: Total number of campaigns accepted.

Age: Calculated as 2025 - Year_Birth.

Simplified categories:

Combined similar education levels into one.

Merged marital statuses into 'Relationship' and 'Single'.
📁 To Save Cleaned File

df.to_csv("cleaned_marketing_campaign.csv", index=False)
