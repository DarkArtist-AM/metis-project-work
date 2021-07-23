##**Metis Business Student Project Description**

#**Potential Client(s):**

 Government-run State Hospitals

#**Abstract:** 

Due to the Pandemic, hospitals have had to deal with a large influx of new patients. At this time, it is evermore important that hospitals keep a pulse on their patients' experiences with hospital care so that hospitals might maintain or improve upon their reputations. I seek to adivse Government-run state hospitals on the areas most highly related to patient experiences above the (national) average. These kinds of hospitals in particular rank lower than the national average more often then not. 

#**Data:**

The data used for my analysis will be a spreadsheet of hospital information. The spreadsheet is 4813 rows by 29 columns. Along with general information on the name, whereabouts, and type of Hospital for all 4813 hospitals recorded in the data, the spreadsheet also keeps information on how each hospital compares to the national average in mortality, safety of care, readmission, effectiveness of care, timliness of care, and effective use of medical imaging. (Also provides some footnotes for the 6 categories mentioned.)

data: https://www.kaggle.com/cms/hospital-general-information (can be downloaded here as a csv file)

note: the target variable and several other columns have values that are one of three strings: "below the national average", "same as the national average", "above the national average".

**#Data Cleaning Considerations:**

1. Dataset is fairly tidy. Each hospital seems to have unique identifer called ProviderID. (Should perhaps double-check the uniqueness of ProviderID just incase.)

2. There are potential missing values, labeled 'Not Available'. We should replace these with Null values and then remove them. 
3. For each of the 6 types of categorical data (mentioned above), each variable is written in two columns - one that contains the actual descriptive data and the other that contains additional explanation if the original value was not given or 'Not Available' in this sense. It seems that the only explanation for a value that does not have any available data will state 'Results are not available for this reporting...'. Thus, I will likely toss out any columns that have "footnote" in their title to make the dataset easier to read. (That is, footnotes dont seem to be adding any valuable information.)

 **#Desired Impact**: 

Help identify areas of great importance on the typical patient experience in order to better accomodate patients in a difficult time. 

**#Impact Hypothesis:**

I believe several of the categories mentioned above will have a demonstrably significant impact on whether the patient experience was below, the same, or above the national average. 

**#Solution Path:**

-Build a classification model to demonstrate the impact of certain features on patient experience.

Steps:

1. Clean data for null values and irrelevant columns
2. Change data types of relevant columns
3. Factorize relevant variables into dummy variables (hospital ownership, hospital type)
4. Build xgb classification model for the data to test the importance of each feature on "Patient experience national comparison" (target variable)



**#Tools:**

-Excel for data analysis and manipulation

-Python (Pandas library and matplotlib)

-Tableau for visualization