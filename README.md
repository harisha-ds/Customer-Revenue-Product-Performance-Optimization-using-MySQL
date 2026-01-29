Customer Revenue & Product Performance Optimization (SQL Project)    

Project Overview :      
This project analyzes sales, customer, and product data for an e-commerce business using MySQL to uncover key revenue drivers, customer behavior patterns, and product performance insights.         
The goal is to support data-driven business decisions related to pricing, promotions, customer retention, and regional strategy.      

Business Problem:      
The e-commerce company faces:     
Uneven revenue growth across regions    
Unclear impact of discounts on revenue   
Limited visibility into customer loyalty and repeat purchases   
Difficulty identifying top-performing products and suppliers     
Management needs SQL-based insights to guide strategic decisions.         

Business objectives:   
-- Identify top revenue-generating products and categories   
-- Evaluate the effectiveness of discounts on sales and revenue    
-- Analyze customer loyalty and repeat purchase behavior    
-- Understand regional and payment method performance    
-- Rank products and customers using advanced SQL techniques  

Domain: 
E-Commerce / Retail Analytics   

Stakeholders:   
Sales Manager   
Marketing Team         
Product Manager      
Business Leadership       

Tools & Technologies:         
Database: MySQL     
Query Language: Advanced SQL       
Data Cleaning: Excel          
Data Model: Relational (3 tables)     
Dataset Size: ~3,000 records       

Dataset Description:    
The analysis is based on three relational tables:     
sales_data        
Order details, revenue, quantity, discounts, delivery status, dates       
customer_info    
Customer demographics, loyalty tier, purchase frequency      
product_info        
Product details, category, supplier, launch date       

Data Model Design:      
Primary keys defined on all master tables    
Foreign key relationships:   
One customer → many orders     
One product → many orders  
Designed to mirror real-world enterprise transactional systems     
A final analytics view was created by joining all three tables to enable reusable analysis    

Data Cleaning & Preparation:          
Removed missing and invalid values using Excel      
Standardized column names and data types     
Resolved data import issues in MySQL     
Removed orphan records to maintain referential integrity   
Validated joins and calculations after modeling   

SQL Techniques Used:   
Multi-table joins  
Aggregations & grouping  
Conditional logic (CASE WHEN)  
Subqueries  
Window functions (RANK, ROW_NUMBER, SUM() OVER)   
Views for reusable analytics 
Date-based analysis & trends   

Business Questions Answered: 

Revenue & Product Analysis   
Total revenue generated   
Revenue by product category   
Top-selling products by quantity   
Top-performing regions by revenue   
Revenue by payment method   

Customer & Behavior Analysis   
Number of unique customers   
Repeat customer identification   
Average order value by loyalty tier   
Revenue per customer by loyalty tier   
Revenue contribution from repeat customers   

Discounts, Operations & Conditional Analysis   
Discounted vs non-discounted revenue comparison   
Quantity differences with discounts   
Regional response to discounts   
Revenue impact of delivery status   
Cancellation rates by payment method  

Advanced Product Performance      
Products with above-average revenue    
Products contributing to top 20% of revenue (Pareto analysis)   
Performance of newer vs older products   
Supplier-wise revenue contribution    
Products performing well in some regions but poorly in others   

Advanced SQL Analysis             
Rank products within each category    
Identify top 3 products per category    
Cumulative revenue contribution 

Customer-level analysis:   
Total revenue per customer    
Customer ranking by spending    
Identify customers spending above their loyalty-tier average  

Data Modeling & Reusability   
Created a final analytics view combining sales, customer, and product data    
Derived:              
Monthly revenue trends     
Category-wise growth        

Seasonality and demand spikes    
Built reusable queries for:     
Monthly top customer monitoring    
Revenue contribution summaries   

Insights & Recommendations:      
1. Revenue & Category Performance
Insights  
Total revenue: ₹261,334.96  
Revenue concentrated in a few categories   
Cleaning products lead revenue; Personal Care underperforms   
Recommendations   
Focus inventory and promotions on high-performing categories   
Reassess pricing and assortment for low-performing categories   
Allocate more budget to high-performing regions     

2. Customer Behavior & Loyalty   
Insights  
Repeat customers contribute a large share of revenue    
Higher loyalty tiers generate more revenue per customer   
Missing loyalty data limits deeper analysis    
Recommendations   
Strengthen loyalty and retention programs   
Encourage loyalty enrollment at checkout   
Improve customer data capture   

3. Discount Effectiveness   
Insights   
Discounts increase quantity purchased   
Discounts do not always increase revenue per order   
Recommendations   
Use targeted, selective discounts   
Evaluate both revenue and margin impact   

4. Regional Discount Performance   
Insights    
Discount effectiveness varies significantly by region   
Recommendations    
Implement region-specific discount strategies   
Redesign or reduce discounts in low-response regions   

5. Delivery & Operations   
Insights    
Delivered orders generate most revenue    
Certain payment methods show higher cancellations   
Recommendations    
Improve order validation and fulfillment   
Optimize high-cancellation payment methods   

6. Product & Supplier Performance   
Insights  
Few products and suppliers generate most revenue   
Strong Pareto (80/20) effect observed   
Some products perform well only in specific regions   
Recommendations   
Prioritize high-performing products and suppliers   
Apply region-specific pricing and promotions   
Review underperforming products  

7. New vs Existing Products  
Insights   
Older products generate higher revenue   
New products show slower adoption   
Recommendations   
Increase visibility for new products   
Bundle new products with popular items   

8. High-Value Customers   
Insights   
Small group of customers contributes disproportionately high revenue   
Recommendations   
Introduce VIP programs   
Track customer lifetime value (CLV)   

9. Time-Based Trends   
Insights   
Monthly revenue shows seasonality and spikes   
Recommendations   
Align marketing and inventory planning with peak months   
Use trends for demand forecasting  

Conclusion:  
This project demonstrates how advanced SQL analysis can solve real-world business problems by transforming raw transactional data into actionable insights.   
