# 📱 Cellphone Company Power BI Dashboard

## 🧩 Project Overview
This Power BI project analyzes cellphone brands, models, and customer ratings to uncover insights about pricing, performance, and consumer behavior.  
The dashboard provides interactive filters and visuals for exploring different aspects such as brand rating, gender distribution, release year trends, and pricing comparisons.

---

## 🧹 Data Cleaning & Transformation
Data cleaning was performed using **Power Query Editor** in Power BI.

### 🔧 Applied Steps:
1. **Source** – Loaded the raw dataset into Power BI.  
2. **Promoted Headers** – Promoted the first row to column headers.  
3. **Changed Type** – Converted columns to appropriate data types (text, numeric, date).  
4. **Added Custom Column** – Created new calculated columns for derived metrics.  
5. **Multiplied Column** – Performed numeric transformations for price normalization.  
6. **Changed Type1** – Finalized column data types after transformations.

These steps ensured data accuracy, consistency, and readiness for analysis.

---

## 📐 DAX Calculations
The following key measures were created using **DAX (Data Analysis Expressions)** in Power BI:

```DAX
-- Average Price
Avg Price = AVERAGE(Cellphones[Price])

-- Average Rating
Avg Rating = AVERAGE(Cellphones[Rating])

-- Number of Unique Brands
Unique Brands = COUNTROWS(VALUES(Cellphones[Brand]))

-- Number of Unique Models
Unique Models = COUNTROWS(VALUES(Cellphones[Model]))
