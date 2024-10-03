# 📊 Walmart Sales Data Analysis - SQL Project

## 🌟 Introduction
Dive into the fascinating world of retail sales! This project analyzes Walmart's sales data to uncover patterns, identify high-performing branches and products, and enhance sales strategies. By understanding customer behavior, we aim to provide actionable insights that can optimize business performance.

## 🎯 Project Objectives
- **Identify** high-performing branches and products.
- **Analyze** sales patterns across various product lines.
- **Understand** customer behavior to refine sales strategies.

## 📈 Data Overview
The dataset is sourced from the **Kaggle Walmart Sales Forecasting Competition** and includes sales transactions from three Walmart branches in **Mandalay, Yangon,** and **Naypyitaw**. The dataset contains **1,000 rows** and **17 columns**, including:

| Column               | Description                             | Data Type        |
|----------------------|-----------------------------------------|-------------------|
| 🧾 `invoice_id`      | Invoice of the sales made               | VARCHAR(30)       |
| 🏪 `branch`          | Branch at which sales were made         | VARCHAR(5)        |
| 🌆 `city`            | The location of the branch              | VARCHAR(30)       |
| 👥 `customer_type`   | The type of the customer                | VARCHAR(30)       |
| 🚻 `gender`          | Gender of the customer                  | VARCHAR(10)       |
| 📦 `product_line`    | Product line of the product sold        | VARCHAR(100)      |
| 💲 `unit_price`      | Price of each product                   | DECIMAL(10, 2)    |
| 📊 `quantity`        | Amount of the product sold              | INT               |
| 💰 `VAT`             | Amount of tax on the purchase           | FLOAT(6, 4)       |
| 🛒 `total`          | Total cost of the purchase              | DECIMAL(12, 4)    |
| 📅 `date`            | Date of purchase                        | DATETIME          |
| ⏰ `time`            | Time of purchase                        | TIME              |
| 💳 `payment`         | Total amount paid                       | DECIMAL(10, 2)    |
| 📉 `cogs`           | Cost Of Goods Sold                      | DECIMAL(10, 2)    |
| 📈 `gross_margin_pct`| Gross margin percentage                  | FLOAT(11, 9)      |
| 💵 `gross_income`    | Gross Income                             | DECIMAL(12, 4)    |
| ⭐ `rating`          | Customer rating                         | FLOAT(2, 1)       |

## 🔍 Analysis Approach
1. **Data Wrangling**: Examine data for NULL or missing values and handle them effectively.
2. ## 🔧 Feature Engineering
   To enhance the analysis, we generated new columns from existing data:

   - **`time_of_day`**: This column categorizes sales into **Morning**, **Afternoon**, and **Evening**, providing insights into which part of the day most sales occur.
   - **`day_name`**: This column extracts the day of the week from the transaction date (Mon, Tue, Wed, Thu, Fri), helping identify the busiest days for each branch.
   - **`month_name`**: This column extracts the month from the transaction date (Jan, Feb, Mar), allowing us to determine which month has the highest sales and profits.

3. **Exploratory Data Analysis (EDA)**: Comprehensive analyses to answer key business questions.

## ❓ Key Business Questions
### 🔍 Generic Questions
- How many distinct cities are present in the dataset?
- In which city is each branch situated?

### 📦 Product Analysis
- How many distinct product lines are there in the dataset?
- What is the most common payment method?
- What is the most selling product line?
- What is the total revenue by month?
- Which month recorded the highest Cost of Goods Sold (COGS)?
- Which product line generated the highest revenue?
- Which city has the highest revenue?
- Which product line incurred the highest VAT?
- Add a column `product_category`, indicating 'Good' or 'Bad' based on sales performance.
- Which branch sold more products than the average?
- What is the most common product line by gender?
- What is the average rating of each product line?

### 💰 Sales Analysis
- Number of sales made in each time of the day per weekday?
- Identify the customer type that generates the highest revenue.
- Which city has the largest VAT?
- Which customer type pays the most VAT?

### 👥 Customer Analysis
- How many unique customer types does the data have?
- How many unique payment methods does the data have?
- Which is the most common customer type?
- Which customer type buys the most?
- What is the gender of most of the customers?
- What is the gender distribution per branch?
- Which time of the day do customers give most ratings?
- Which time of the day do customers give most ratings per branch?
- Which day of the week has the best avg ratings?
- Which day of the week has the best average ratings per branch?

## ✨ Unique Insights
Discoveries from this analysis highlight peak evening sales during local festivals, allowing for targeted promotions. Additionally, underperforming product lines were identified for data-driven improvements.

## 🚀 Conclusion and Future Work
This analysis lays the groundwork for enhanced sales strategies at Walmart. Future work could include applying machine learning models to predict sales trends based on historical data.

## 🤝 Collaboration
I welcome feedback and insights from the community. Let’s enhance this analysis together!


