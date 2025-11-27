# Sales Analytics Project

## 1. Executive Summary
This project operationalizes a full-stack sales analytics pipeline using MySQL for data ingestion, cleaning, and analysis, complemented by business intelligence dashboards for executive reporting. The objective is to transform raw sales data into actionable insights that support revenue optimization, customer segmentation, and operational decision-making.

---

## 2. Project Objectives
- Centralize and structure transactional sales data.
- Build analytical queries to evaluate performance indicators.
- Generate visual dashboards that communicate business trends.
- Demonstrate end-to-end data engineering and analytics workflow.

---

## 3. Folder Structure




---

## 4. Dataset Description
The dataset contains three major domains:

### **customers.csv**
- `customer_id`
- `customer_name`
- `email`
- `phone`
- `region`

### **products.csv**
- `product_id`
- `product_name`
- `category`
- `unit_price`

### **orders.csv**
- `order_id`
- `customer_id`
- `product_id`
- `order_date`
- `quantity`
- `total_amount`

---

## 5. Data Dictionary (Detailed)
| Table | Column | Description |
|-------|---------|-------------|
| customers | customer_id | Unique customer identifier |
| customers | customer_name | Full name |
| customers | email | Customer email |
| customers | phone | Phone number |
| customers | region | Region of customer (North, South, East, West) |
| products | product_id | Unique product identifier |
| products | product_name | Product name |
| products | category | Product category |
| products | unit_price | Price per product unit |
| orders | order_id | Unique order identifier |
| orders | customer_id | FK → customers |
| orders | product_id | FK → products |
| orders | order_date | Date of purchase |
| orders | quantity | Units sold |
| orders | total_amount | Revenue from the order |

Place this in `docs/data_dictionary.md`.

---

## 6. How to Run the Project

### **Step 1 — Create the database**
```sql
CREATE DATABASE sales_analytics;
USE sales_analytics;

