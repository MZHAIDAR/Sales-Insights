## Sales Insights Data Analysis Project

![image](https://github.com/MZHAIDAR/Sales-Insights/assets/99173615/d659b83b-7b0c-4089-88d7-bafd7e9304fc)

![image](https://github.com/MZHAIDAR/Sales-Insights/assets/99173615/33f37ed8-abab-4478-bb78-182cf8a0d6a0)

![image](https://github.com/MZHAIDAR/Sales-Insights/assets/99173615/a7f643cd-f6ba-4977-93b6-255f6c0b4339)




### Data Analysis Using SQL

1. Show all customer records

    `SELECT * FROM customers;`

1. Show total number of customers

    `SELECT count(*) FROM customers;`

1. Show transactions for Chennai market (market code for chennai is Mark001

    `SELECT * FROM transactions where market_code='Mark001';`

1. Show distrinct product codes that were sold in chennai

    `SELECT distinct product_code FROM transactions where market_code='Mark001';`

1. Show transactions where currency is US dollars

    `SELECT * from transactions where currency="USD"`

1. Show transactions in 2020 join by date table

    `SELECT transactions.*, date.* FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020;`

1. Show total revenue in year 2020,

    `SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.currency="INR\r" or transactions.currency="USD\r";`
	
1. Show total revenue in year 2020, January Month,

    `SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and and date.month_name="January" and (transactions.currency="INR\r" or transactions.currency="USD\r");`

1. Show total revenue in year 2020 in Chennai

    `SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020
and transactions.market_code="Mark001";`


Data Analysis Using Power BI
============================

### Steps and ideas involved
1.  Uploading sales data to Mysql and analysis.

2.  Connecting data with PowerBI and Transforming and cleansing the data.

3.  Joining The data Table and creating Dashboard.

4.  Analysing Total revenue and sales quantity.

5.  Also analysing sales and revenue on the basis of year ,month ,Market.

6.  Also examining top 5 cumtomer and product on the basis of sales quantity.

#### Profit analysis

6.  Analysing total profit on the basis of year,month, market.
7.  Analysing revenue contributionin % by markets.
8.  Analysing margin %  by market.
9.  Also the its profit contribution in % to the total profit.

    
### Key insights

