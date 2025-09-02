# Sales Performance Analysiss using PowerBI

## Objective:

This project focuses on analyzing transactional sales data to uncover key insights into revenue patterns across different regions, sales representatives, product categories, and customer segments. By leveraging Excel’s Power Query, we transformed raw sales data into a clean, structured format suitable for insightful analysis.

The ultimate goal is to help stakeholders identify:

- Top-performing regions and sales reps

- Product category trends

- Customer behavior patterns

- Sales performance over time

##
## Data Overview

The dataset represents individual sales transactions across both online and retail channels, covering a range of product categories. Each row corresponds to a single transaction, including sales, customer, and product details.

| Column Name            | Description                                                              |
| ---------------------- | ------------------------------------------------------------------------ |
| `Product_ID`           | Unique identifier for each product                                       |
| `Sale_Date`            | Date of the sale                                                         |
| `Sales_Rep`            | Name of the sales representative involved in the transaction             |
| `Region`               | Sales region (e.g., North, South, East, West)                            |
| `Sales_Amount`         | Total revenue from the transaction                                       |
| `Quantity_Sold`        | Number of units sold                                                     |
| `Product_Category`     | Category of the product (e.g., Furniture, Food, Electronics, Clothing)   |
| `Unit_Cost`            | Cost per unit (Removed for this analysis)                                |
| `Unit_Price`           | Selling price per unit (Removed for this analysis)                       |
| `Customer_Type`        | Customer type – New or Returning                                         |
| `Discount`             | Discount applied (decimal format, e.g., 0.1 for 10%)                     |
| `Payment_Method`       | Payment method used (Cash, Credit Card, Bank Transfer, etc.)             |
| `Sales_Channel`        | Whether the sale was Online or Retail                                    |
| `Region_and_Sales_Rep` | Combined field of Region and Sales Representative (for grouped analysis) |

##
## Data Preparation (Power Query)

The dataset was cleaned and transformed using Power Query in Microsoft Excel to ensure it was ready for analysis. The following steps were taken:

**1. Removed Unnecessary Columns**

- Removed: **Unit_Cost** , **Unit_Price**
  
These were excluded as the focus of this analysis is on revenue trends, not profit margins or unit economics.
##

**2.reated New Time-Based Columns**

Extracted:

- Year → from Sale_Date

- Month_Name → full name of the month (e.g., February, March)

These fields enable seasonality and time-based trend analysis.
##

**3. Converted Data Types**

Converted the following fields to text format to support grouping and consistent reporting:

- Product_ID → Text

- Discount → Text

- Year → Text
##

**4. Cleaned & Validated**

- Ensured correct data types across columns

- Checked for and confirmed the absence of:

     - ***Duplicate entries***

     - ***Null or missing values***
 
##
## Analysis Performed

The cleaned dataset was analyzed with Sales Amount as the primary metric. Key dimensions of the analysis included:

***1. Region-wise Sales***

  - Identified which regions are generating the most revenue.

***2. Sales Representative Performance***

  - Compared individual sales reps to find top performers.

***3. Product Category Trends***

   - Analyzed which product categories contribute most to revenue.

***4. Seasonal Trends***

  - Analyzed monthly and yearly sales trends using the derived Year and Month_Name columns.

***5. Payment Method Preferences***

  - Looked into which payment methods are preferred by customers.

***6. Channel Analysis***

  - Compared Online vs Retail sales performance.
##

## Report
<img width="1342" height="747" alt="image" src="https://github.com/user-attachments/assets/3161af24-bdff-4fd7-82b7-070022152d68" />

##
## Conclusion

This sales analysis provided meaningful insights into regional performance, product popularity, and customer behavior. The use of Power Query ensured clean, structured, and analyzable data forming the foundation for impactful business decisions.

