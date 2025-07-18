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
    <img width="1366" height="746" alt="17528689043982055339339770962674" src="https://github.com/user-attachments/assets/247e6e67-b2e1-48c3-bc1d-0212728272ea" />

2. Pivot Table
    - Table1: Average Discount percentage by Product Category
    - Table 2: Product count by Product Category.
    - Table 3: sum of rating count by product category.
    - Table 4: Top 10 products name by average Rating
    - Table 5:Average actual price vs Discounted price by category.
    - Table 6:Top 5 products in terms of Average Rating_count
    - Table 7:Count of product by rating.
    - Table 8: Count of product by High discount(50% or more discount).
   
    <img width="439" height="133" alt="17528673583986658582602600530983" src="https://github.com/user-attachments/assets/1ae3203f-d791-40c5-b3c2-adfd418bd74c" />
   - Table 8: Count of products by rating.
   - Table 9: Sum of Potential revenue by Category.
   - Table 10: Count of Category by Price range bucket.
   - Table 11: Average of Rating by Discount Level.
   - Table 12: Count of Products by Low Review.
   - Table 13: Top 5 Average of Discount percentage by Product Category.
   - Table 14: Top 5 Average Rating by Product.
<img width="1180" height="536" alt="17528687913045118634721265710963" src="https://github.com/user-attachments/assets/d110cdb8-6f02-4bb9-af7d-58b6ef1d7e40" />

3. Creating of Dashboard

<img width="1344" height="694" alt="17528686327998707364661137765611" src="https://github.com/user-attachments/assets/bb56b313-47ca-4a88-b792-4f427b8e9ac8" />
