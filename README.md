# DSA Documentation
This is where I started my portfolio building with my Data Analysis project work in the Incubator Hub.
## Project Topic: Amazon-Product-Review-Analysis
### Project Overview
This Data Analysis Project aims to generate insight from Amazon Product review by its Customer. By analysing the various parameters in the data received we seek to  gather enough insight to guide product improvement, marketing strategies and customer engagement.
### Tools Used
Microsoft Excel
  - Power Query Editor for Data cleaning.
  - Ms Excel worksheet for Pivot Table, Charts, and Dashboard.
### Data Description 
- Source:Amazon product review data
- Fields included:
  - Product name
  - Category
  - Actual price & Discounted price
  - Discount %
  - Rating
  - Rating Count
  - Review content
  - Low Review
  - High Discount
  - Potential Revenue
- Total no of product: 1,34
- Total Products Category: 9
- Total Potential Revenue: $113.64bn
- Total actual price: $8M
- Total Discount price:$4M
### Exploratory Data Analysis 
1. What is the average discount percentage by product category?
2. How many products are listed under each category?
3. What is the total number of reviews per category?
4. Which products have the highest average ratings?
5. What is the average actual price vs the discounted price by category?
6. Which products have the highest number of reviews?
7. How many products have a discount of 50% or more?
8. What is the distribution of product ratings (e.g., how many products are rated 3.0,
4.0, etc.)?
9. What is the total potential revenue (actual_price × rating_count) by category?
10. What is the number of unique products per price range bucket (e.g., <₹200,₹200–₹500, >₹500)?
11. How does the rating relate to the level of discount?
12. How many products have fewer than 1,000 reviews?
13. Which categories have products with the highest discounts?
14. Identify the top 5 products in terms of rating and number of reviews combined.
#### Steps to Analysis Solutions 
1. Data Cleaning with Power Query Editor:
  - Removing of all Data excesses from the product name and product Category.
  -  Removing of duplicate from Product_id to make it unique.
  - Adding of Custom Column: Potential Revenue= [actual price]*[rating_count]
  - Adding of conditional Column:
    - Price Bucket Range= if [discounted_price]<200 then "200" else if [discounted price] <=500 then "200-500" else "500"
    - Low Review= if [rating_count] <1000 then "yes" else "No"no
    - Discounted Level= if [discount_percentage] <=0.1 then "0%-10%" else if [discount percentage]<=0.2 then "11%-20%" if ... else "91%-100%".
2. Pivot Table
 1. Table1: Average Discount percentage by Product Category
  <img width="418" height="267" alt="17528662168836285276004937953476" src="https://github.com/user-attachments/assets/19fe2cd7-4e78-4212-bbf4-3e1508ab6a7d" />
2. Table 2: Product count by Product Category.
    
 4. Table 3: Total rating count by product category.
 5. 
