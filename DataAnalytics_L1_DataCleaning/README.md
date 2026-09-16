\# Cafe Sales Data Cleaning



\## Oasis Infobyte - Data Analytics Internship

\### Level 1 - Task 3: Cleaning Data



\## Project Overview



This project focuses on cleaning a messy Cafe Sales dataset and transforming it into a clean, consistent, and analysis-ready dataset using Python and Pandas.



The dataset contained missing values, duplicate records, invalid placeholder values, incorrect data types, and other data quality issues that required systematic cleaning and validation.



\## Tools \& Technologies



\- Python

\- Pandas

\- NumPy

\- Jupyter Notebook



\## Data Cleaning Process



The following steps were performed:



1\. Loaded and inspected the dataset.

2\. Assessed missing values, duplicates, and data types.

3\. Removed duplicate records.

4\. Replaced invalid `ERROR` and `UNKNOWN` placeholders.

5\. Converted numerical columns to appropriate data types.

6\. Converted Transaction Date to datetime format.

7\. Recovered missing numerical values using:

&#x20;  - Total Spent = Quantity × Price Per Unit

&#x20;  - Known item prices where appropriate

8\. Handled remaining missing categorical values using `Unknown`.

9\. Removed records where essential numerical or date information could not be reliably recovered.

10\. Checked categorical values for formatting inconsistencies.

11\. Detected outliers using the IQR method.

12\. Retained valid high-value transactions identified as statistical outliers.

13\. Validated the relationship between Quantity, Price Per Unit, and Total Spent.

14\. Exported the final cleaned dataset.



\## Data Quality Improvement



| Metric | Before Cleaning | After Cleaning |

|---|---:|---:|

| Row Count | 10,020 | 9,514 |

| Missing Values | 6,834 | 0 |

| Duplicate Rows | 20 | 0 |

| ERROR Placeholders | 1,627 | 0 |

| UNKNOWN Placeholders | 1,638 | 0 |



\## Outlier Analysis



The IQR method was used to identify potential outliers.



No outliers were detected in Quantity or Price Per Unit.



For Total Spent, 259 values were identified above the IQR upper limit. Further inspection showed that these represented valid transactions. Therefore, these values were retained rather than removed or capped.



\## Validation



The final dataset was validated using the relationship:



\*\*Total Spent = Quantity × Price Per Unit\*\*



The validation resulted in \*\*0 mismatched records\*\*, confirming numerical consistency.



\## Final Result



The final cleaned dataset contains:



\- \*\*9,514 rows\*\*

\- \*\*8 columns\*\*

\- \*\*0 missing values\*\*

\- \*\*0 duplicate rows\*\*

\- \*\*0 ERROR placeholders\*\*

\- \*\*0 UNKNOWN placeholders\*\*



The cleaned dataset is ready for further analysis and visualization.



\## Project Structure



\- `Dataset/` - Raw/working Cafe Sales dataset

\- `Notebook/` - Jupyter Notebook containing the complete cleaning process

\- `Outputs/` - Final cleaned Cafe Sales CSV

\- `Screenshots/` - Screenshots of important cleaning and validation results



\## Conclusion



This project demonstrates a structured data-cleaning workflow involving data quality assessment, missing-value treatment, duplicate removal, data type correction, logical value recovery, categorical data handling, outlier detection, validation, and final dataset export.

