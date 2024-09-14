# Super market-Sales-Data Cleaning and Analysis

## Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools Used](#tools-used)
- [Data Cleaning/Preparation - using Python](#data-cleaning/preparation---using-python)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Results and Findings](#results-and-findings)
- [Limitations](#limitations)
    - [Data Quality Issues](#data-quality-issues)
    - [Data Tideness Issues](#data-tideness-issues)

## Project Overview

This data analysis project aims to provide insights into the sales performance of a Super market over the first quarter in 2019. By analyzing various aspects of the sales data, we seek to identify trends, make data-driven recommendations, and gain a deeper understanding of the super market performance.

### Revenue Page
![Revenue Page](https://github.com/user-attachments/assets/93715432-d02a-48e1-a430-4c205b30601c)

### Revenue Page with Visualization Tooltip
![Revenue Page with a visualization tooltip](https://github.com/user-attachments/assets/29f76df6-44eb-4d57-8b9d-3027cbdbb733)

### Revenue by Month Page
![Revenue by month Page](https://github.com/user-attachments/assets/05429766-89b8-4a47-8d88-646e2cdc2177)

### Revenue by Day Page
![Revnue by day Page](https://github.com/user-attachments/assets/8e663291-5816-4ef9-9d83-373dc9beed05)

### Revenue by Day Page with Visualization Tooltip
![Revenue by day Page with a visualization tooltip](https://github.com/user-attachments/assets/c8a7ebbe-3974-4c95-87b9-2a87b2ad6869)

### Rating and Statistics Page
![Rating   Statistics Page](https://github.com/user-attachments/assets/aecd7370-f504-4143-a4ce-b98e22ebbff8)



## Data Sources
Sales Data: The primary dataset used for this analysis is the "Capstone Data - Supermarket Sales.csv" file, containing detailed information about each invoice of the sale made by customers.

## Tools used
- Python : Data Wrangling 

- PowerBi : Data Visualization 
    - [Download the tool](https://www.microsoft.com/en-us/download/details.aspx?id=58494) 

## Data Cleaning/Preparation - using Python
In the initial data preparation phase, we performed the following tasks:
1. Data loading and inspection.
2. Handling missing values.
3. Data cleaning and formatting. 

## Exploratory Data Analysis
exploring the sales data to answer key questions, such as:
- What is the total number of invoices?
- What is the total revenue?
    - The total revenue by each city.
    - The total revenue by day and city.
    - The total revenue by each product line and gender.
    - The total revenue by time.
    - The total revenue by day of week.
    - The total revenue by month and [Customer type/Payment].
- What is the Average Rating?
    - What is the average rating for each city?
- What is the total number of customers by sex/Customer type?
- What is the most used payment method? e.g: Cash , wallet , etc..

## Results and Findings
The analysis results are summarized as follows:
1. #### Total Revenue: 
The total revenue for the first quarter of 2019 amounts to 323,000 USD.

2. #### Top City by Revenue: 
Naypyitaw recorded the highest revenue among all cities analyzed.\
    *Note:* All the cities are mostly equal.  

3. #### City with Highest Rating: 
Naypyitaw also received the highest average customer rating.
    *Note:* All the cities are mostly equal.


4. #### Peak Sales Time: 
The analysis shows that 7:00 PM is the peak hour for traffic and sales.

5. #### Top Revenue Month: 
The month of January recorded the highest revenue during the period examined.

6. #### least Revenue Month:
The month of February recorded the least revenue during the period examined.\
    *Note:* February has decreased revenue by **16%**


7. #### Customer Type Revenue Comparison: 
Supermarkets generated more revenue from normal customers than from members.\
    *Note:* Although Customer type has no effect on the revenue


8. #### Top Revenue Day:
Saturdays produced the highest revenue compared to other days of the week.

9. #### Best-Selling Product Line:
The Food & Beverages category emerged as the most sold product line.

10. #### Customer Type Distribution: 
The number of normal customers exceeded the number of member customers.

11. #### Gender Distribution: 
The count of male customers was higher than that of female customers.

12. #### Most Preferred Payment Method: 
E-wallets accounted for the largest percentage of payments among the various methods.\
    *Note:* All payment methods are mostly equal.


## Limitations
### Data Quality Issues
1. Drop the duplicated rows
2. Rating column values should be between 0 and 10.
    - multiply any rating value bigger than 10 with (0.1) to get the exact rating.
3. Remove any characters from the Unit Price Column values to be only numerical values.
4. Convert all Unit Price Column values to float.
5. convert any negative value in Quanitity column to positive.
6. Evaluate the 5% Tax column again to remove all the null values in that column.
7. Rounding the values in the 'Tax 5%' and 'Total' columns to four decimal places for precision.  
8. convert the time string in Time column into a 24-hour time format (HH:MM).
9. Replace value "Memberr" with the correct one "Member"
10. Assuming that the '-' CsutomerType corresponds to "Normal" Customer typed people. Replaced value "-" with the "Normal" customerType.
### Data Tideness Issues
1. Made a new column 'City' which has values {Yangon , Naypyitaw , Mandaly}
2. Drop Yangon , Naypyitaw , Mandaly this columns.
3. Merge the 'City' and 'Branch' columns.
4. Drop 'City' and 'Branch' columns.
