## **Retail Sales and Customer Insights: A Comprehensive SQL Analysis**  

### **Introduction**  
This project analyzes customer purchasing behavior, product sales trends, and order performance using MySQL. The goal is to extract meaningful insights that can help businesses optimize inventory management, improve customer engagement, and maximize revenue.  

### **Dataset Overview**  
The dataset consists of three tables:  
- **Customers (200 records)** – Includes customer details such as name, email, phone number, city, and country.  
- **Products (50 records)** – Contains product details such as name, category, price, and stock quantity.  
- **Orders (800 records)** – Stores order transactions, including customer purchases, product details, quantity, and order amount.  

These tables are linked using:  
- `CustomerID` (associates orders with customers)  
- `ProductID` (associates orders with products)  

### **Database Schema**  
#### **Customers Table**  
| Column Name   | Data Type        | Description            |  
|--------------|----------------|------------------------|  
| CustomerID   | INT (PK)        | Unique customer ID    |  
| CustomerName | VARCHAR(255)    | Customer's full name  |  
| Email        | VARCHAR(255)    | Email address         |  
| Phone        | VARCHAR(50)     | Contact number        |  
| City         | VARCHAR(100)    | City of residence     |  
| Country      | VARCHAR(100)    | Country of residence  |  

#### **Products Table**  
| Column Name   | Data Type         | Description             |  
|--------------|-----------------|-------------------------|  
| ProductID    | INT (PK)         | Unique product ID       |  
| ProductName  | VARCHAR(255)     | Name of the product     |  
| Category     | VARCHAR(100)     | Product category        |  
| Price        | DECIMAL(10,2)    | Product price           |  
| StockQuantity | INT             | Available stock quantity |  

#### **Orders Table**  
| Column Name   | Data Type         | Description            |  
|--------------|-----------------|------------------------|  
| OrderID      | INT (PK)         | Unique order ID        |  
| CustomerID   | INT (FK)         | Customer who placed the order |  
| ProductID    | INT (FK)         | Ordered product        |  
| Quantity     | INT              | Number of items ordered |  
| OrderAmount  | DECIMAL(10,2)    | Total order amount     |  
| OrderDate    | DATE             | Date of order placement |  

---

## **Data Preprocessing**  
Before analysis, the following data preprocessing steps were performed:  
- Checking for missing values and handling them appropriately  
- Validating data types for consistency  
- Ensuring foreign key integrity between tables  
- Removing duplicate records  
- Normalizing data for efficiency  

---

## **SQL Analysis**  

### **Basic Level Queries**  
1. Retrieve all available products  
2. Count total number of customers  
3. Count total number of products  
4. Find the total revenue from orders  
5. Retrieve customer details from a specific city  
6. Get product details where the price is greater than $500  
7. Find distinct cities where customers are registered  
8. Find the maximum, minimum, and average price of products  
9. Retrieve the most expensive product  
10. Retrieve the cheapest product  
11. Fetch all orders placed in the last 30 days  
12. Get the total number of customers from each country  
13. Find total revenue per month for 2024  
14. List orders sorted by highest order amount  
15. Retrieve the order details where quantity is more than 2  

### **Intermediate Level Queries**  
16. List all customers who placed at least one order  
17. Find customers who have never placed an order  
18. Find the total amount spent by each customer  
19. Find the top 5 customers based on total spending  
20. Find the top 3 most ordered products  
21. Find the least ordered product  
22. Retrieve the total revenue per product category  
23. Retrieve the total number of orders per customer  
24. Find the total revenue generated per city  
25. Find products that were never ordered  
26. Retrieve the total stock by category available in the store  
27. Find products with less than 20 stock quantity  
28. Find orders where the order amount is greater than the average order amount  
29. Retrieve all orders placed in the last 6 months with total amount spent per customer  
30. Find the number of orders placed per month in the last year  

### **Advanced Level Queries**  
31. Find the top 3 customers who placed the highest number of orders  
32. Find the month with the highest total sales  
33. Retrieve customers who placed orders in every month of the last year  
34. Find the product that generated the highest revenue  
35. Retrieve customers who ordered at least 3 different products  
36. Find the first and last purchase date for each customer  
37. Find the percentage of revenue contributed by each product category  
38. List products along with their sales count  
39. Identify the most frequently ordered category  
40. Retrieve customers whose total spending exceeds the average spending of all customers  

---

## **Business Insights**  
From the SQL queries, the following insights were derived:  
- **Customer Segmentation** – Identify high-value customers based on spending patterns.  
- **Product Performance** – Determine best-selling and underperforming products.  
- **Sales Trends** – Identify peak sales months and customer purchasing behaviors.  
- **Inventory Management** – Detect low-stock products requiring replenishment.  
- **Revenue Optimization** – Analyze which product categories generate the most revenue.  

---

## **Conclusion and Recommendations**  
### **Summary**  
This project demonstrates how MySQL can be used to analyze retail sales data and customer behavior. The structured approach enables data-driven decision-making for business growth.  

### **Recommendations**  
- Focus marketing efforts on high-value customers.  
- Increase stock for best-selling products.  
- Offer discounts on slow-moving products.  
- Engage with customers who have not made recent purchases.  
- Optimize inventory based on seasonal trends.  

---

## **Future Scope**  
This study can be extended by:  
- Implementing predictive analytics using machine learning.  
- Integrating real-time dashboards with Power BI or Tableau.  
- Expanding the dataset with additional customer demographics for deeper analysis.  

---

## **Created By**  
ABHISHEK V NIKAM  

---
