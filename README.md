# Blinkit Sales Report

### Dashboard Link : https://app.powerbi.com/reportEmbed?reportId=e1588b76-60af-439f-bf9d-44142683f78b

###

![Screenshot 2024-09-11 153756](https://github.com/user-attachments/assets/6b1feebf-0a43-4257-b6d5-60a25ad15655)

## Problem Statement

This project involves an in-depth analysis of Blinkit sales data to uncover patterns and insights that can drive business decisions. The primary focus is on understanding sales trends, identifying high-performing products, and analyzing customer buying behavior. This report is aimed at helping stakeholders make data-driven decisions to enhance profitability, improve customer experience, and optimize inventory management.

It focuses on total sales, avg sales, avg rating for different outlets across the country.


### Column Breakdown
Item Fat Content:

* Represents whether the item is low-fat or regular-fat.Useful for understanding consumer preferences based on dietary choices.

Item Identifier:

* A unique code for each item. Helps in tracking individual items across various outlets.

Item Type:

* The category of the item (e.g., Food, Drinks, Household). Important for segmenting sales by item categories.

 Outlet Establishment Year:

* The year when the outlet was established. Useful for analyzing how outlet age affects sales performance.

 Outlet Identifier:

* A unique code for each outlet. Helps in tracking sales and performance across different outlets.

 Outlet Location Type:

* The location of the outlet (e.g., Urban, Suburban, Rural). Provides insights into how sales differ by geographic areas.

Outlet Size:

* The size of the outlet (e.g., Small, Medium, Large). This can be used to analyze how outlet size influences sales volumes.

Outlet Type:

* The type of outlet (e.g., Grocery Store, Supermarket) Useful for understanding performance by type of retail environment.

Item Visibility:

* A measure of how much an item is displayed to customers. Can help analyze how item visibility correlates with sales.

Item Weight:

* The weight of each item. Useful for cost and logistics analysis, as heavier items may have higher shipping or handling costs.

Sales:
* The total sales for each item. The most critical column for analyzing overall performance, trends, and revenue contributions by item and outlet.

Rating:
* Could be customer feedback or a quality score. Helps analyze how product quality or customer satisfaction impacts sales.
## Potential Analysis
### Sales Trends:

By item type, fat content, and outlet type.
Analyze how customer preferences vary by product categories and health-conscious choices (fat content).

### Outlet Analysis:

Compare sales across outlets of different sizes and locations.
Determine whether older or newer outlets perform better in sales.

### Customer Behavior:

Understanding how visibility and fat content influence consumer buying behavior.
Analyzing high-performing items and their characteristics (e.g., fat content, weight).

### Regional Performance:

Evaluate the impact of outlet location types on sales (urban vs. rural outlets).
Assess whether location and outlet type correlate with sales success.

### Product and Outlet Matching:

Analyze which types of products perform best in specific outlets.
Identify trends where certain product types (e.g., low-fat items) perform well in specific outlet types (e.g., supermarkets vs. grocery stores).


for creating new column following DAX expression was written;
       
        METRICS = {
    ("Avg sales", NAMEOF('BlinkIT Grocery Data'[Avg Sales]), 1),
    ("Total sales", NAMEOF('BlinkIT Grocery Data'[Total sales]), 0),
    ("No of items", NAMEOF('BlinkIT Grocery Data'[NO of items]), 2),
    ("Avg Rating", NAMEOF('BlinkIT Grocery Data'[Avg Rating]), 3)",
        }
       
        
Snap of cards
##

![Screenshot 2024-09-14 193335](https://github.com/user-attachments/assets/7d0b6bb9-fcb6-4bea-99d4-02e4d9515a00)






        

-----
##
 

## Snapshot of Dashboard (Power BI Service)

![Screenshot 2024-09-14 194323](https://github.com/user-attachments/assets/f045156a-6eb2-4f4a-be75-e825c90fe008)


 

# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### [1] Total Sales

   The total sales amount is $1.20M across all items and outlets.
           
### [2] Average Sales and Ratings

* Average Sales per item is $141.
* Average Rating across items is 3.9, indicating moderate customer satisfaction.
  
  ### [3] Item Distribution
  
* Number of Items: A total of 8,523 unique items were sold.
* Top Item Categories by Sales:
    Fruits and Vegetables and Snacks are the top-selling categories, each contributing $0.18M to total sales.
    Household, Frozen Foods, and Dairy follow, each generating between $0.10M and $0.14M in sales.
* Lowest-selling categories: Items like Seafood, Breakfast items, and Starchy foods generated the lowest sales.

 ### [4] Fat Content Breakdown
 
 * Low Fat products generated $425.36K, while Regular fat items contributed $776.32K in sales.
* Regular-fat items have a larger share of total sales, indicating customer preference for regular-fat products.
 
 ### Fat Content by Outlet Tier
 
* Tier 3 outlets lead in both Low Fat and Regular fat sales:
    Regular Fat: $0.31M
    Low Fat: $0.17M
* Tier 2 and Tier 1 follow closely, but Tier 3 dominates.
         
### Sales by Outlet Establishment Year

* Sales show a significant spike in recent years, with $205K sales in the most recent year shown.
* Earlier years, especially before 2015, saw lower sales, averaging between $78K and $133K.

### Sales by Outlet Size

* High-sized outlets generated the majority of sales, amounting to $507.90K.
* Medium-sized outlets followed, with $248.99K.
* Small-sized outlets accounted for the least sales, at $444.79K.

### Sales by Outlet Location

* Tier 3 locations contributed the highest sales, generating $472.13K (around 71.3% of total sales).
* Tier 2 and Tier 1 locations contributed $393.15K and $336.40K, respectively.

### Sales by Outlet Type

* Supermarket Type 1 outlets dominate sales, generating $787.55K in total.
* Grocery Stores follow with $151.94K in sales.
* Supermarket Type 3 generated $130.71K, while Supermarket Type 2 contributed $131.48K.

Average Sales:
* Grocery stores have the highest average sales per item ($140), closely followed by Supermarket Type 3 and Type 2.

Item Visibility:
* Items in Supermarket Type 1 have the highest visibility (338.65), likely contributing to higher sales.
