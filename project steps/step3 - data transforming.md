# Ferns and Petals Sales Analysis

## Step 3: Data Transformation

### Project Overview
This project analyzes the sales data of **Ferns and Petals (FNP)** to understand:
- Customer behavior
- Sales trends
- Product performance
- Delivery efficiency
- Occasion-based sales

After extracting and cleaning the datasets, the next step is **Data Transformation** using **Power Query Editor (PQE)**.

Data transformation helps create new columns, format data correctly, calculate delivery metrics, and prepare the dataset for modelling and dashboard analysis.

---

# Purpose of Data Transformation

The main objectives of data transformation are:
- Convert incorrect data types
- Create calculated columns
- Extract month and hour information
- Calculate delivery duration
- Merge datasets
- Prepare data for analysis

---

# Open Power Query Editor (PQE)

1. Open Excel
2. Go to:
   **Data → Queries & Connections**
3. Open the required query
4. Click:
   **Transform Data**

Now the dataset opens inside **Power Query Editor (PQE)**.

---

# Transformation in customer.csv

## Convert Contact Number into Text Format

### Steps

1. Open:
   **customer.csv**
2. Select:
   **Contact_Number** column
3. Go to:
   **Transform → Data Type**
4. Select:
   **Text**

---

# Purpose

Contact numbers are converted into text format because phone numbers are only used to identify customers, not for calculations like addition or subtraction.

If the contact number is kept as a number, Excel may:
- Remove starting zeros
- Change the format automatically
- Show the number incorrectly

By converting it into text format:
- The phone number stays exactly the same
- Leading zeros are preserved
- Data formatting problems are avoided
  
---

# Transformation in orders.csv

## Create Month Column from Order Date

### Steps

1. Open:
   **orders.csv**
2. Select:
   **Order_Date** column
3. Go to:
   **Add Column → Date → Month → Name of Month**

---

## Purpose

A Month column is created from the Order_Date column to understand sales performance month by month.

It helps to:
- Analyze monthly sales
- Compare revenue across different months
- Identify high and low sales months
- Apply month-wise filters in the dashboard

---

## Output

A new column is created:

| Order_Date | Month |
|---|---|
| 2023-01-15 | January |
| 2023-02-10 | February |

---

# Create Hour Column from Order Time

### Steps

1. Select:
   **Order_Time** column
2. Go to:
   **Add Column → Time → Hour**

---

## Purpose

An Hour column is created from the Order_Time column to understand at what time customers place orders.

It helps to:
- Identify peak ordering hours
- Understand customer buying patterns
- Find the busiest time of the day
- Analyze customer activity by hour
---

## Output

A new column is created:

| Order_Time | Hour |
|---|---|
| 10:45 AM | 10 |
| 07:30 PM | 19 |

---

# Calculate Delivery Duration

### Steps

1. Select:
   **Delivery_Date** column
2. Go to:
   **Add Column → Custom Column**
3. Create formula:

```text
Delivery_Date - Order_Date
```

4. Click **OK**

---

## Purpose

Delivery duration is calculated to understand how much time is taken to deliver an order after it is placed.

It helps to:
- Analyze delivery performance
- Measure delivery efficiency
- Calculate average delivery days
- Identify delayed deliveries
- Improve customer satisfaction

---

## Convert Duration into Days

### Steps

1. Select the newly created duration column
2. Go to:
   **Transform → Duration → Days**

---

## Purpose

The delivery duration is converted into days to make the delivery time easier to understand and analyze.

It helps to:
- Measure how many days delivery takes
- Compare delivery speed for different orders
- Calculate average delivery days
- Identify slow or delayed deliveries

---

## Output

| Order_Date | Delivery_Date | Delivery_Days |
|---|---|---|
| 01-Jan-2023 | 03-Jan-2023 | 2 |

---

# Create Hour Column from Delivery Time

### Steps

1. Select:
   **Delivery_Time** column
2. Go to:
   **Add Column → Time → Hour**

---

## Purpose

A Delivery Hour column is created from the Delivery_Time column to understand at what time orders are delivered.

It helps to:
- Analyze delivery timing patterns
- Identify preferred delivery hours
- Understand customer delivery preferences
- Track busiest delivery times

---

## Output

| Delivery_Time | Delivery_Hour |
|---|---|
| 08:00 AM | 8 |
| 06:30 PM | 18 |

---

# Merge Queries with products.csv

### Steps

1. Open:
   **orders.csv**
2. Go to:
   **Home → Merge Queries**
3. Select:
   **products.csv**
4. Match columns using:
   - Product_ID
5. Click:
   **OK**

---

# Extract Product Price

After merging:

1. Expand merged table
2. Select:
   - Price (INR)
3. Click:
   **OK**

Now the price column is added into the orders table.

---

## Purpose

The products table is merged with the orders table to combine product details with order information.

It helps to:
- Extract product prices into the orders table
- Calculate total revenue for each order
- Prepare data for sales analysis and dashboard creation

---

# Load Transformed Data

After completing all transformations:

1. Click:
   **Home → Close & Load To**
2. Select:
   - Table
   OR
   - Data Model
3. Click:
   **OK**

---

# Benefits of Data Transformation

- Improves analytical capability
- Enables monthly sales analysis
- Helps calculate delivery metrics
- Supports dashboard filtering
- Enhances business insights

---

# Expected Outcome

After completing this step:
- New analytical columns are created
- Delivery metrics are calculated
- Product prices are merged successfully
- Data becomes ready for modelling and dashboard creation

---

# Tools Used

- Microsoft Excel
- Power Query Editor (PQE)
- Merge Queries
- Custom Columns
- Date Functions
- Time Functions

---

# Next Steps

After data transformation, continue with:

1. Data Modelling
2. Data Analysis
3. Pivot Tables & Measures
4. Dashboard Creation
5. Executive Summary

---

# Conclusion

Data Transformation helps convert raw data into an analysis-ready format. Using Power Query Editor features such as custom columns, merge queries, date transformations, and duration calculations improves the quality of analysis and prepares the dataset for dashboard development.
