***Purposes Of The Project***

The major aim of thie project is to gain insight into the sales data of Walmart to understand the different factors that affect sales of the different branches.

***About Data***

The dataset was obtained from the Kaggle Walmart Sales Forecasting Competition(https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting). This dataset contains sales transactions from a three different branches of Walmart,
respectively located in Mandalay, Yangon and Naypyitaw. The data contains 17 columns and 1000 rows:

| Column                   | Description                                   | Data Type          |
|--------------------------|-----------------------------------------------|--------------------|
| `invoice_id`             | Invoice of the sales made                     | `VARCHAR(30)`      |
| `branch`                 | Branch at which sales were made               | `VARCHAR(5)`       |
| `city`                   | The location of the branch                    | `VARCHAR(30)`      |
| `customer_type`          | The type of the customer                      | `VARCHAR(30)`      |
| `gender`                 | Gender of the customer making purchase        | `VARCHAR(10)`      |
| `product_line`           | Product line of the product sold              | `VARCHAR(100)`     |
| `unit_price`            | The price of each product                     | `DECIMAL(10, 2)`   |
| `quantity`               | The amount of the product sold                | `INT`              |
| `VAT`                    | The amount of tax on the purchase             | `FLOAT(6, 4)`      |
| `total`                  | The total cost of the purchase                | `DECIMAL(10, 2)`   |
| `date`                   | The date on which the purchase was made       | `DATE`             |
| `time`                   | The time at which the purchase was made       | `TIMESTAMP`        |
| `payment_method`         | The total amount paid                         | `DECIMAL(10, 2)`   |
| `cogs`                   | Cost Of Goods Sold                            | `DECIMAL(10, 2)`   |
| `gross_margin_percentage`| Gross margin percentage                       | `FLOAT(11, 9)`     |
| `gross_income`           | Gross Income                                  | `DECIMAL(10, 2)`   |
| `rating`                 | Rating                                        | `FLOAT(2, 1)`      |


1.**Product Analysis**
Conduct analysis on the data to understand the different product lines, the products lines performing best and the product lines that need to be improved.

2.**Sales Analysis**
This analysis aims to answer the question of the sales trends of product. The result of this can help use measure the effectiveness of each sales strategy
the business applies and what modificatoins are needed to gain more sales.

3.**Customer Analysis**
This analysis aims to uncover the different customers segments, purchase trends and the profitability of each customer segment.

**Approach Used**

1.**Data Wrangling**:  
I.NULL values and missing values are detected and data replacement methods are used to replace, missing or NULL values.

II.Built a database :Created table and inserted the data.

II.Select columns with null values in them. There are no null values in our database as in creating the tables, we set NOT NULL for each field, hence null values are filtered out.

2.**Feature Engineering**:
HERE we generate some new columns from existing ones.

I.Add a new column named time_of_day to give insight of sales in the Morning, Afternoon and Evening. This will help answer the question on which part of the day most sales are made.

II.Add a new column named day_name that contains the extracted days of the week on which the given transaction took place (Mon, Tue, Wed, Thur, Fri). This will help answer the question on which week of the day each branch is busiest.

II.Add a new column named month_name that contains the extracted months of the year on which the given transaction took place (Jan, Feb, Mar). Help determine which month of the year has the most sales and profit.

IV.Exploratory Data Analysis (EDA): Exploratory data analysis is done to answer the listed questions and aims of this project.


**Generic Questions we answered in this** 

How many unique cities does the data have?

In which city is each branch?

**Relating to Product**

How many unique product lines does the data have?

What is the most common payment method?

What is the most selling product line?

What is the total revenue by month?

What month had the largest COGS?

What product line had the largest revenue?

What is the city with the largest revenue?

What product line had the largest VAT?

Fetch each product line and add a column to those product line showing "Good", "Bad". Good if its greater than average sales

Which branch sold more products than average product sold?

What is the most common product line by gender?

What is the average rating of each product line?

**Sales**

Number of sales made in each time of the day per weekday

Which of the customer types brings the most revenue?

Which city has the largest tax percent/ VAT (Value Added Tax)?

Which customer type pays the most in VAT?

**Customer**

How many unique customer types does the data have?

How many unique payment methods does the data have?

What is the most common customer type?

Which customer type buys the most?

What is the gender of most of the customers?

What is the gender distribution per branch?

Which time of the day do customers give most ratings?

Which time of the day do customers give most ratings per branch?

Which day fo the week has the best avg ratings?

Which day of the week has the best average ratings per branch?
