# Analyzing-Amazon-Product-Review.
 A data analysis project focused on Amazon product reviews using Microsoft Excel. This project includes data cleaning, pivot tables, review counts by category, discount percentage analysis, and dashboard creation for insights into product performance 
 ## What I Learned in This Data Analysis Training

Throughout this Data Analysis training program, I have developed strong foundational skills in tools such as Microsoft Excel and Power BI, which I used extensively to carry out this Amazon Product Review Analysis.

### ✅ Excel
I learned how to clean and structure raw data, use formulas like IF, COUNTIF, AVERAGEIFS, and create Pivot Tables to summarize and explore large datasets. I also created calculated columns to support deeper analysis and used charts to visualize insights effectively.

### ✅ Power BI
Power BI has helped me learn how to transform data using Power Query, build interactive dashboards, and use visuals like bar charts, pie charts, and slicers to explore data across multiple fields. It also improved my storytelling and helped me communicate findings clearly.



### 🧠 SQL (Still Learning)
Although I am still working on fully understanding SQL, I’ve been introduced to its importance in querying databases, filtering data, and extracting insights using SELECT, WHERE, and GROUP BY statements. I look forward to mastering SQL as I continue practicing.

Overall, this training has given me confidence in using data to uncover trends, solve problems, and support decision-making. This project is my first step toward becoming a professional data analyst.
## Project Topic:E-commerce analytics solution
## Project Overview
As a beginner in data analysis, this project marks the completion of my training in Microsoft Excel, Power BI, and introductory SQL. The purpose of this capstone project is to apply the skills I have learned in a real-world scenario by analyzing Amazon product review data.
I was given a dataset containing various information about products sold on Amazon, including their names, categories, prices, ratings, and customer reviews. My task was to explore the dataset, clean and organize it using Excel, analyze patterns using pivot tables and formulas, and finally present my findings with a dashboard.
This project has helped me gain practical experience in working with raw data, drawing conclusions from patterns, and creating visual insights that support business decisions. It also reflects my understanding of the foundational tools used by data analysts.

## Project Objectives
The main objective of this project was to carry out an Exploratory Data Analysis (EDA) on a dataset from Amazon using Microsoft Excel and Power BI. As someone new to data analysis, this project gave me the opportunity to practice using Pivot Tables, calculated fields, and charts to solve real business problems.

The specific business questions I was expected to answer include:
1. What is the average discount percentage by product category?
2.  How many products are listed under each category?
3. What is the total number of reviews per category?
4.  Which products have the highest average ratings?
5. What is the average actual price vs. discounted price by category?
6. Which products have the highest number of reviews?
7. How many products have a discount of 50% or more?
8. What is the distribution of product ratings (e.g., how many products are rated 3.0, 4.0, etc.)?
9. What is the total potential revenue (actual price × rating count) by category?
10. What is the number of unique products per price range bucket (e.g., <₹200, ₹200–₹500, >₹500)?
11. How does the rating relate to the level of discount?
12. How many products have fewer than 1,000 reviews?
13. Which categories have products with the highest discounts?
14. Identify the top 5 products in terms of rating and number of reviews combined.
Completing this project has helped me to understand how data is used to answer real business questions and how Excel can be used as a powerful analysis tool.

🔸 Q1. What is the average discount percentage by product category?
Tool Used: Pivot Table
Steps:
Insert Pivot Table
Rows: Category
Values: Average of Discount %
Insight: Categories like "Fashion" and "Electronics" had higher average discounts, indicating they may be more competitive or frequently promoted.

🔸 Q2. How many products are listed under each category?
Tool Used: Pivot Table
Steps:
Rows: Category
Values: Count of Product Name
Insight: The “Books” category had the most product listings, showing a wide variety in that segment.

🔸 Q3. What is the total number of reviews per category?
Tool Used: Pivot Table
Steps:
Rows: Category
Values: Sum of Review Count
Insight: “Electronics” had the highest review count, suggesting higher customer engagement.

🔸 Q4. Which products have the highest average ratings?
Tool Used: Sort in Excel
Steps:
Sort the Rating column from Largest to Smallest
Insight: The top-rated products all had a 5.0 average, but with few reviews. High rating + high review count is more reliable.

🔸 Q5. What is the average actual price vs the discounted price by category?
Tool Used: Pivot Table
Steps:
Rows: Category
Values: Average of Actual Price and Average of Discounted Price
Insight: “Home Appliances” had the highest original price but offered significant discounts.

🔸 Q6. Which products have the highest number of reviews?
Tool Used: Sort in Excel
Steps:
Sort the Review Count column from Largest to Smallest
Insight: The top-reviewed products were mostly in “Electronics” and “Home & Kitchen.”

🔸 Q7. How many products have a discount of 50% or more?
Tool Used: New Column + Pivot Table
Steps:
1. Add a column:
=IF([@[Discount %]]>=50, "Yes", "No")
2. Pivot Table:
Rows: Discount ≥ 50%
Values: Count of Product Name
Insight: Over 400 products had a 50% or more discount — major promotions.

🔸 Q8. What is the distribution of product ratings (e.g., how many products are rated 3.0, 4.0, etc.)?
Tool Used: Pivot Table
Steps:
Rows: Rating
Values: Count of Product Name
Insight: Most products were rated between 4.0 and 4.5 — generally positive feedback.

🔸 Q9. What is the total potential revenue (Actual Price × Rating Count) by category?
Tool Used: Calculated Column + Pivot Table
Steps:
1. Add a column:
=Actual Price * Rating Count
2. Pivot Table:
Rows: Category
Values: Sum of Revenue
Insight: “Electronics” had the highest potential revenue.

🔸 Q10. What is the number of unique products per price range bucket (e.g., <₹200, ₹200–₹500, >₹500)?
Tool Used: Helper Column + Pivot Table
Steps:
1. Create a bucket column:
=IF([Actual Price]<200, "<₹200", IF([Actual Price]<=500, "₹200–₹500", ">₹500"))

🔸 Q11. How does the rating relate to the level of discount?
Tool Used: Scatter Chart
Steps:
X-axis: Discount %
Y-axis: Rating
Insight: No strong direct relationship — products with high discounts don't always have high or low ratings.

🔸 Q12. How many products have fewer than 1,000 reviews?
Tool Used: COUNTIF
Formula:
=COUNTIF([Review Count], "<1000")
Insight: A majority of products had under 1,000 reviews, showing they may be new or niche.

🔸 Q13. Which categories have products with the highest discounts?
Tool Used: Pivot Table
Steps:
Rows: Category
Values: Max of Discount %
Insight: Categories like "Fashion" and "Beauty" had products with the steepest discounts (up to 80–90%).

🔸 Q14. Identify the top 5 products in terms of rating and number of reviews combined.
Tool Used: New Column + Sort
Steps:
1. Add a column for "combined score":
=Rating + (Review Count / 1000)
2. Sort this column from largest to smallest.
Insight: Products with high ratings and high review counts were top performers, mostly in “Electronics” and “Home Essentials.”

In conclusion I'm grateful for this oppurtunity to be part of this training and this project helped me apply what I’ve learned in Excel and Power BI to real data. I now feel more confident analyzing datasets, answering business questions, and presenting insights visually. I look forward to improving my SQL skills and continuing my data analysis journey.
























