DAX-Data-Visualization – Power BI

Project Overview

This project focuses on analyzing sales data using Microsoft Power BI. The report includes data modeling, DAX calculations, and interactive visualizations to understand sales, profit, orders, targets, products, categories, and geographic performance.

Data Tables

The main tables used in the project are:

List of Orders – Contains order-level information such as Order ID, order date, customer/location details, and state.

Order Details – Contains sales transaction details such as Order ID, Amount, Profit, Category, and Sub-Category.

Sales Target – Contains sales targets by category.

Data Relationships

The following relationships are established:

List of Orders → Order Details

Relationship column: Order ID

Order Details → Sales Target

Relationship column: Category

The relationship should be active.

DAX Calculations

Total Sales

Total Sales = SUM('Order Details'[Amount])

Order Count

Order Count = DISTINCTCOUNT('List of Orders'[Order ID])

Other Calculations

The project also includes calculations such as:

Profit Margin

Sales Category

Average Profit in Delhi

Revenue per Order

Sales and target comparisons

Minimum target by segment

Visualizations

1. Sales Performance Matrix

A Matrix visual is used to analyze actual sales against sales targets across different categories and months.

Suggested fields:

Rows: Category

Columns: Month

Values: Total Sales and Sales Target

This helps compare actual performance with planned targets.

2. Total Sales Amount and Sales Target

Use Card visuals to display:

Total Sales Amount

Sales Target

A Multi-row Card can be used to display the minimum target for each segment.

3. Comparison of Profit and Quantity

Use an appropriate comparison visual to analyze Profit and Quantity across categories or other relevant dimensions.

4. Geographic Sales Analysis

A Map visual is used to visualize total sales by city and identify regional sales patterns.

Suggested fields:

Location: City

Size: Total Sales or Amount

Legend: State (optional)

Tooltips: Order ID or other relevant information (optional)

The City column should be categorized as City under:

Column tools → Data category → City

If locations are not recognized correctly, State and Country information can be used to improve geographic identification.

5. Sales Distribution by Sub-Category

A Treemap is used to represent sales distribution across different sub-categories.

Suggested fields:

Category: Sub-Category

Values: Total Sales or Amount

Larger rectangles represent sub-categories with higher sales.

6. Order Count Analysis by State

A Funnel Chart is used to visualize the distribution of order counts across different states.

Suggested fields:

Category: State

Values: Order Count

States with larger sections have a higher number of orders.

7. Monthly Sales Trend

A Line Chart is used to show the trend of monthly sales over time.

Suggested fields:

X-axis: Order Date / Date hierarchy / Month

Y-axis: Total Sales

If the dataset covers multiple years, use Year and Month together to avoid combining the same month from different years.

Key Analysis Objectives

The Power BI report is designed to answer questions such as:

What is the total sales amount?

How do actual sales compare with sales targets?

Which categories and sub-categories generate the most sales?

Which cities have the highest sales?

Which states have the highest number of orders?

How do monthly sales change over time?

How do profit and quantity vary across categories?

What is the minimum target for each segment?

What is the average profit for orders placed in Delhi?

Report Features

The dashboard can include:

Interactive slicers

Cards

Multi-row cards

Matrix

Map

Treemap

Funnel chart

Line chart

Bar/column charts

Tooltips and cross-filtering

Tools Used

Microsoft Power BI Desktop

Power Query

DAX

Excel/CSV sales data

Conclusion

This Power BI project provides an interactive view of sales performance from multiple perspectives. The combination of DAX measures, relationships, and visualizations makes it possible to analyze sales trends, geographic performance, order distribution, category performance, and target achievement efficiently.
