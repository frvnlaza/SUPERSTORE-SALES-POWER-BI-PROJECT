The goal of this project is to model and analyze data from a sales records database for scale model cars and then extract information for decision-making. You've been tasked with producing a report that answers a set of questions below:

- What were the total sales for the company?
- What were the profits by segment? Which segment has the most profit?


The Super Store dataset contains data on order details of customers for orders of a superstore in the U.S.

It contains 13 columns:

-	Order ID: all order IDs
-	Customer ID: all customer information
-	Customer Name: customer name
-	Segment: segments of product
-	Country: country of sales
-	Market: continent/market of sales
-	Product ID: list of product IDs
-	Category: category of different product
-	Sub-Category: sub-category of product
-	Product Name: product name
-	Sales: sales of different product
-	Quantity: quantity of product sale
-	Profit: profit made

### Data Cleaning
By inspecting the dataset, we discovered some issues:

1.	The current header isn't meaningful. The first row contains data, and the second row should be the header. 
-	You'll have to remove the first row and then promote the second row as the header.
2.	There is a discrepancy between the columns' content and their data types. 
3.	The format of the Date column values isn't consistent. It has two different delimiters. Some of them use the dd-mm-yyyy format, and others use dd/mm/yyyy.
- You'll have to replace all / by - to format all dates the same way.

### Analysis
After cleaning the dataset and removing inconsistencies, let's now add some columns for analysis. We're interested in making our analysis on different date granularity, such as year and month. Therefore, we'll add two columns to our table.

What were the total sales for the company?
- To answer this question, we'll compute the total sales and visualize it. Let's create a new measure for that. 


![image](https://github.com/frvnlaza/SUPERSTORE-SALES-POWER-BI-PROJECT/assets/140290612/343a94b3-79b1-436f-bc9e-6c5330341b2f)

What were the profits by segment? 
- To answer these questions, let's find the net profit for all customer segments (Consumer, Corporate, and Home Office) in 2016.

Which segment has the most profit?
- The Consumer segment has the most profit.


![image](https://github.com/frvnlaza/SUPERSTORE-SALES-POWER-BI-PROJECT/assets/140290612/d7f4435e-f619-49e0-8d3c-346e2d6d63be)


