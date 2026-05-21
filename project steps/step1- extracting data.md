# Ferns and Petals Sales Analysis

## Step 1: Extract Data

### Project Overview
This project analyzes the sales data of **Ferns and Petals (FNP)** to understand:
- Customer behavior
- Sales trends
- Product performance
- Delivery efficiency
- Occasion-based sales

The first step in this project is **Data Extraction**, where all CSV datasets are imported into the analysis tool(Excel).

---

# Dataset Details

The project contains 3 datasets:

---

## 1. customer.csv

This file contains customer-related information.

### Columns
- Customer_ID
- Name
- City
- Contact_Number
- Email
- Gender
- Address

---

## 2. products.csv

This file contains product-related information.

### Columns
- Product_ID
- Product_Name
- Category
- Price (INR)
- Occasion
- Description

---

## 3. orders.csv

This file contains order transaction details.

### Columns
- Order_ID
- Customer_ID
- Product_ID
- Quantity
- Order_Date
- Order_Time
- Delivery_Date
- Delivery_Time
- Location
- Occasion

---

# How to Extract Data

## Option 1: Using Excel / Power Query Editor (PQE)

### Step 1: Download Dataset Files
Download all CSV files and place them inside one folder.

Files:
- customer.csv
- products.csv
- orders.csv

---

### Step 2: Import Data into Excel

1. Open **Microsoft Excel**
2. Create a **New Workbook**
3. Go to:

   **Data → Get Data → From File → From Folder**

4. Select the folder containing:
   - customer.csv
   - products.csv
   - orders.csv

5. Click **Open**

---

### Step 3: Open Power Query Editor (PQE)

1. After selecting the folder, Excel will display files in **Binary Format**
2. Click on **Transform Data**

This opens the **Power Query Editor (PQE)** tool.

---

### Step 4: Convert Binary Files into Tables

1. Select the **Binary** cell of the file
2. Right-click on it
3. Click:

   **Add as New Query**

4. Double-click the file in the **Properties Section**
5. Change:
   - Path → File Name

Example:
- customer.csv
- products.csv
- orders.csv

Repeat the same process for all files.

---

# Next Steps

After data extraction, continue with:

1. Data Cleaning
2. Data Transformation
3. Data Modelling
4. Data Analysis
5. Pivot Tables & Measures
6. Dashboard Creation
7. Executive Summary

---

# Expected Outcome

After completing this step:
- All datasets will be imported successfully
- Data will be ready for cleaning and transformation
- Tables will be connected using relationships
- The dashboard development process can begin

---

# Tools Used

- Microsoft Excel
- Power Query Editor (PQE)
- Power Pivot
- Pivot Tables
  
---

# Conclusion

The Data Extraction step is the foundation of the project. Properly importing and organizing the datasets ensures accurate analysis and effective dashboard creation for Ferns and Petals Sales Analysis.
