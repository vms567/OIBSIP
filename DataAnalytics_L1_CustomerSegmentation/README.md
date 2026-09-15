\# Customer Segmentation Analysis



\## Oasis Infobyte - Data Analytics Internship

\### Level 1 - Task 2



\## Project Overview



This project focuses on analyzing customer purchasing behavior and segmenting customers into meaningful groups using RFM (Recency, Frequency, Monetary) analysis and K-Means clustering.



The objective is to identify different types of customers based on their purchasing patterns and provide actionable marketing strategies for each customer segment.



\## Dataset



The project uses the \*\*Online Retail Dataset\*\* from the UCI Machine Learning Repository.



The dataset contains transactional data from a UK-based online retail company and includes information such as:



\- Invoice Number

\- Stock Code

\- Product Description

\- Quantity

\- Invoice Date

\- Unit Price

\- Customer ID

\- Country



Original dataset size: \*\*541,909 rows and 8 columns\*\*.



\## Tools and Technologies



\- Python

\- Pandas

\- NumPy

\- Matplotlib

\- Seaborn

\- Scikit-learn

\- Jupyter Notebook



\## Project Workflow



\### 1. Data Loading and Inspection

\- Loaded the Online Retail dataset using Pandas.

\- Examined dataset structure, data types, missing values, duplicates, and descriptive statistics.



\### 2. Data Cleaning

\- Removed transactions with missing Customer IDs.

\- Removed duplicate records.

\- Identified and excluded cancelled transactions.

\- Removed transactions with zero or negative quantity and unit price.

\- Created `TotalPrice` using Quantity × UnitPrice.



After cleaning, \*\*392,692 valid transaction records\*\* remained.



\### 3. RFM Analysis



Customer purchasing behavior was analyzed using:



\- \*\*Recency:\*\* Number of days since the customer's most recent purchase.

\- \*\*Frequency:\*\* Number of unique purchases made by the customer.

\- \*\*Monetary:\*\* Total amount spent by the customer.



A total of \*\*4,338 customers\*\* were included in the RFM analysis.



\### 4. Data Transformation and Scaling



The RFM variables showed skewness, particularly Frequency and Monetary.



A logarithmic transformation was applied to reduce skewness, followed by `StandardScaler` to standardize the features before clustering.



\### 5. Elbow Method



The Elbow Method was used to determine an appropriate number of clusters.



Based on the reduction in inertia, \*\*K = 3\*\* was selected for customer segmentation.



\### 6. K-Means Customer Segmentation



K-Means clustering divided the customers into three segments:



| Segment | Customers | Avg. Recency | Avg. Frequency | Avg. Monetary |

|---|---:|---:|---:|---:|

| High-Value Customers | 769 | 17.06 | 13.35 | 7898.46 |

| At-Risk Customers | 1872 | 167.36 | 1.35 | 361.00 |

| Regular Customers | 1697 | 44.20 | 3.38 | 1259.58 |



\## Customer Segment Interpretation



\### High-Value Customers



These customers purchase recently and frequently and have the highest monetary value. They represent the most valuable and loyal customer segment.



\### Regular Customers



These customers demonstrate moderate recency, frequency, and monetary value. They have the potential to become high-value customers through increased engagement.



\### At-Risk Customers



These customers have high recency and low frequency and monetary value. They have not purchased recently and require re-engagement strategies.



\## Marketing Recommendations



\### High-Value Customers

\- Provide loyalty rewards and VIP benefits.

\- Offer exclusive deals and early access to new products.

\- Use personalized recommendations, cross-selling, and upselling.



\### Regular Customers

\- Encourage repeat purchases using personalized offers.

\- Introduce loyalty programs and targeted promotions.

\- Recommend products based on previous purchasing behavior.



\### At-Risk Customers

\- Launch win-back and re-engagement campaigns.

\- Provide limited-time discounts and personalized offers.

\- Use reminders and targeted communication to encourage customers to return.



\## Key Insights



\- At-Risk Customers form the largest segment with \*\*1,872 customers\*\*.

\- Regular Customers represent \*\*1,697 customers\*\* and provide an opportunity for conversion into high-value customers.

\- High-Value Customers consist of \*\*769 customers\*\* and contribute significantly more value through frequent and recent purchases.

\- RFM analysis combined with K-Means clustering provides an effective approach for understanding customer purchasing behavior.



\## Project Structure



DataAnalytics\_L1\_CustomerSegmentation/

\- Dataset/

&#x20; - Online Retail.xlsx

\- Notebook/

&#x20; - Customer\_Segmentation\_Analysis.ipynb

\- Outputs/

&#x20; - cleaned\_online\_retail.csv

&#x20; - customer\_segmentation\_results.csv

\- Screenshots/

&#x20; - Elbow\_Method.png

&#x20; - Customer\_Count\_by\_Segment.png

&#x20; - Recency\_vs\_Frequency.png

&#x20; - Frequency\_vs\_Monetary.png

&#x20; - Recency\_Distribution.png

&#x20; - Frequency\_Distribution.png

&#x20; - Monetary\_Distribution.png

\- README.md



\## Conclusion



This project demonstrates how customer transaction data can be transformed into meaningful customer segments using RFM analysis and K-Means clustering.



The identified segments can help businesses design targeted marketing strategies, improve customer retention, re-engage inactive customers, and increase overall customer value.

