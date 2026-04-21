# PowerBi-data-representation
The project displays data from superstore, which shows customer data from american company
1. Data Cleaning (Power Query)
Removal of Duplicates & Nulls: Ensuring every Customer ID is unique. Handling null "Exit Dates" by replacing them with a placeholder or creating a "Still Employed" flag.
Unpivoting Columns: Our survey data has questions as column headers, i unpivot them to create a "Question" and "Response" column structure.
Conditional Columns: Creation of  custom buckets for "order_count" using if...then...else logic in Power Query.
Date Table Generation: Useage of Power Query to create a dynamic Calendar Table—essential for time-intelligence functions like Year-over-Year growth.

2. Data Modeling (The "Star Schema")
Connecting our cleaned tables. .
Fact Table: customer Records/Transactions.
Dimension Tables: Order date, Department, Location, and order count.

3. Advanced DAX (Measures)
Time-Intelligence: Calculating order discounts compared to the same period last year.
Dynamic Title: Using DAX to create a report title that changes based on the slicer selection("Order date, using the year to distingush").

4. Interactive Visualization

KPI Cards: Total sales, Average Discount, Total Profit.

Tooltips: Created a hidden "Tooltip Page" that shows an yoy percentage
