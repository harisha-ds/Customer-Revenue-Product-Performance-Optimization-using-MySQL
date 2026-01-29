# Customer Revenue & Product Performance Optimization
### SQL Analytics Project | E-Commerce Domain

---

## Executive Summary
This project analyzes **sales, customer, and product data** for an e-commerce business using **MySQL**.  
The objective is to identify **revenue drivers**, evaluate **discount effectiveness**, and understand **customer loyalty behavior**.

Key findings show that:
- A small group of products and customers contributes most of the revenue
- Discounts increase purchase volume but do not always increase revenue
- Regional and payment-method performance varies significantly

---

## Business Problem
The company is experiencing:
- Uneven revenue growth across regions
- Unclear impact of discounts on revenue
- Limited visibility into customer loyalty and repeat purchases
- Difficulty identifying high-performing products and suppliers

Management requires **SQL-based insights** to support strategic decisions.

---

## Business Objectives
- Analyze customer purchases, product performance, and revenue trends
- Identify top-performing products, customers, and regions
- Evaluate the effectiveness of discounts
- Support pricing, promotion, and retention strategies

---

## Domain
**E-Commerce / Retail Analytics**

---

## Tools & Technologies
- **Database:** MySQL  
- **Query Language:** SQL (Advanced)  
- **Data Cleaning:** Excel  
- **Data Model:** Relational  
- **Dataset Size:** ~3,000 records  

---

## Dataset Overview
The analysis is based on **three relational tables**:

### sales_data
- Order details
- Purchase amount, quantity
- Discounts and delivery status
- Transaction date

### customer_info
- Customer demographics
- Loyalty tier
- Purchase frequency

### product_info
- Product details
- Category and supplier
- Launch date

---

## Data Model Design
- Primary keys on all master tables  
- Foreign key relationships:
  - One customer → many orders  
  - One product → many orders  
- Mirrors real-world enterprise transactional databases  
- Created a **final analytics view** for reusable analysis

---

## Data Cleaning & Preparation
- Removed missing and invalid values using Excel  
- Standardized column names and data types  
- Resolved MySQL data import issues  
- Removed orphan records  
- Validated joins and calculations  

---

## SQL Techniques Used
- Multi-table joins  
- Aggregations and grouping  
- `CASE WHEN` conditional logic  
- Subqueries  
- Window functions:
  - `RANK()`
  - `ROW_NUMBER()`
  - `SUM() OVER()`  
- Views for reusable analytics  
- Date-based analysis  

---

## Business Questions Answered

### Revenue & Product Analysis
1. Total revenue generated  
2. Revenue by product category  
3. Top-selling products by quantity  
4. Top-performing regions by revenue  
5. Revenue by payment method  

---

### Customer & Behavior Analysis
1. Number of unique customers  
2. Repeat customer identification  
3. Average order value by loyalty tier  
4. Revenue per customer by loyalty tier  
5. Revenue contribution from repeat customers  

---

### Discounts & Operations Analysis
1. Discounted vs non-discounted revenue  
2. Quantity difference when discounts are applied  
3. Regional response to discounts  
4. Revenue impact of delivery status  
5. Cancellation rates by payment method  

---

### Advanced Product Performance
1. Products with above-average revenue  
2. Top 20% revenue-contributing products (Pareto analysis)  
3. New vs old product performance  
4. Supplier-wise revenue contribution  
5. Regional product performance variation  

---

### Advanced SQL Analysis
- Product ranking within categories  
- Top 3 products per category  
- Cumulative revenue contribution  
- Customer-level revenue and ranking  
- Customers spending above loyalty-tier average  

---

## Key Insights & Recommendations

### Revenue & Category Performance
- Total revenue: **₹261,334.96**
- Revenue concentrated in a few categories
- Cleaning category performs best

**Recommendation:**  
Focus inventory and promotions on high-performing categories and regions.

---

### Customer & Loyalty Impact
- Repeat customers contribute a large share of revenue
- Higher loyalty tiers generate more revenue per customer

**Recommendation:**  
Strengthen loyalty programs and improve customer data capture.

---

### Discount Effectiveness
- Discounts increase order quantity
- Discounts do not always increase revenue per order

**Recommendation:**  
Apply targeted discounts instead of blanket offers.

---

### Product & Supplier Insights
- Strong Pareto effect observed
- Few products and suppliers drive most revenue

**Recommendation:**  
Prioritize high-performing products and suppliers.

---

## Conclusion
This project demonstrates how **advanced SQL analytics** can be used to solve real-world business problems by transforming raw transactional data into **actionable business insights**.

---

## Author
**Harisha Thoparapu**  
Aspiring Data Analyst | SQL | Power BI | Python | Excel | Data Analytics
