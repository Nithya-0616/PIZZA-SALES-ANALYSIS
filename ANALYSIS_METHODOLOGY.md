# Pizza Sales Analysis – Methodology & Technical Documentation

## 1. Project Overview

This project analyses pizza sales data using Microsoft Power BI to understand sales performance, customer ordering patterns, product preferences and revenue trends.

The analysis transforms transaction-level sales data into meaningful business insights through data preparation, DAX calculations, exploratory analysis and interactive visualisations.

## 2. Business Objectives

The primary objectives of this analysis are:

- Evaluate overall revenue and order performance.
- Identify the best-performing pizzas.
- Analyse monthly revenue trends.
- Identify peak ordering hours and days.
- Understand customer preferences across pizza sizes.
- Compare sales performance across pizza categories.
- Identify the most frequently used individual ingredients.

## 3. Dataset Overview

The analysis uses the Pizza Sales dataset.

| Attribute | Details |
|---|---|
| Total records | 48,620 |
| Total columns | 12 |
| Unique orders | 21,350 |
| Total pizzas sold | 49,574 |
| Total revenue | $817,860.05 |
| Average order value | $38.31 |
| Average pizzas per order | 2.32 |
| Analysis period | January–December 2015 |

### Key Dataset Attributes

- `pizza_id` – Unique pizza record identifier.
- `order_id` – Order identifier.
- `pizza_name_id` – Pizza name identifier.
- `quantity` – Number of pizzas ordered.
- `order_date` – Date of the order.
- `order_time` – Time of the order.
- `unit_price` – Price per pizza.
- `total_price` – Total transaction value.
- `pizza_size` – Pizza size.
- `pizza_category` – Pizza category.
- `pizza_ingredients` – Ingredients used in the pizza.
- `pizza_name` – Pizza name.

## 4. Tools and Technologies

**Primary Tool:** Microsoft Power BI

**Supporting Technologies and Techniques:**
- Power Query
- DAX (Data Analysis Expressions)
- Data Cleaning and Transformation
- Data Modelling
- KPI Development
- Data Visualization
- Interactive Dashboard Development

## 5. Data Preparation and Validation

The source dataset was reviewed before performing the analysis.

The validation process included:

- Reviewing the dataset structure and column names.
- Checking the number of records and columns.
- Verifying date and time fields.
- Reviewing numerical fields used in sales calculations.
- Checking missing values and duplicate records.
- Validating revenue and quantity calculations against the source dataset.

### Data Quality Summary

| Validation | Result |
|---|---:|
| Total records | 48,620 |
| Total columns | 12 |
| Missing values | 0 |
| Duplicate rows | 0 |
| Unique order IDs | 21,350 |

## 6. Power Query Transformations

Power Query was used to prepare the data for analysis.

### 6.1 Original Sales Table

The original `PIZZA` table was retained at the transaction level.

An important correction was made during data preparation: an earlier
