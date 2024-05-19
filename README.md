# SQL-project

Write a SQL query that orders the items by price.

SELECT item_name , price
FROM superstore
ORDER BY price DESC;

Write your own SQL query that will show a statistic about the item prices, like a sum, average, minimum, maximum, or count.

SELECT SUM(price) FROM superstore;
SELECT AVG(price) FROM superstore;
SELECT MIN(price) FROM superstore;
SELECT MAX(price) FROM superstore;
SELECT COUNT(price) FROM superstore;

Write your own SQL query that will show a statistic about the price for items in the category of "Kitchen Supplies".

SELECT item_name, price, category
FROM superstore
WHERE category= "Kitchen Supplies";

SELECT SUM(price) category
FROM superstore
WHERE category= "Kitchen Supplies";

SELECT AVG(price) category
FROM superstore
WHERE category= "Kitchen Supplies";

Come up with your own question about the data and try to answer it using SQL. 

List the prices for items in Appliances

SELECT item_name, price, category
FROM superstore
WHERE category=  "Appliances";

What is the sum of the appliances?

SELECT SUM(price) category 
FROM superstore
WHERE category= "Appliances";

What is the stock quantity of items in each category? List in ascending order

SELECT item_name, category, stock_quantity
FROM superstore
ORDER BY stock_quantity ASC;
