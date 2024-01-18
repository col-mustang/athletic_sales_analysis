# athletic_sales_analysis

## Three Goals:
1. Analyze sales data to gain insights into which cities in the U.S. have sold the most athletic wear over two years.
2. Determine which retailers had the greatest total sales for athletic wear, and which retailers sold the most women's athletic footwear. 
3. Determine which day and week had the highest sales for women's athletic footwear.

### File Collection
Starter code ("athletic_sales_analysis_starter_code.jpynb) and sales data for 2020 & 2021 (in separate CSV files) imported.

## Combine and Clean the Data
1. Import the two CSV files, athletic_sales_2020.csv and athletic_sales_2021.csv, and read them into DataFrames.
2. Check that the columns in the two DataFrames have similar names and data types.
3. Combine the two DataFrames by the rows using an inner join, and reset the index.
4. After combining the DataFrames, do the following: 
    - Check if there are any null values.
    - Check each column’s data type.
    - Convert the "invoice_date" column to a datetime data type.
    - Confirm that the data type has been changed.

## Determine which Region Sold the Most Products
1. Use both the groupby and pivot_table function to create a multi-index DataFrame with the "region", "state", and "city" columns.
2. Rename the aggregated column to reflect the aggregation of the data in the column.
3. Sort the results in ascending order to show the top five regions, including the state and city that have the greatest number of products sold. The final table looks like the following image:

    <img src="https://static.bc-edx.com/ai/ail-v-1-0/m5/lms/img/M5-greatest-number-products.png" alt="image" width="50%" height="50%">

## Determine which Region had the Most Sales
1. Use both the groupby and pivot_table function to create a multi-index DataFrame with the "region", "state", and "city" columns.
2. Rename the aggregated column to reflect the aggregation of the data in the column.
3. Sort the results in ascending order to show the top five regions, including the state and city that generated the most sales. The final table looks like the following image:

    <img src="https://static.bc-edx.com/ai/ail-v-1-0/m5/lms/img/M5-most-sales.png" alt="image" width="50%" height="50%">

## Determine which Retailer had the Most Sales
1. Use both the groupby and pivot_table function to create a multi-index DataFrame with the "retailer", "region", "state", and "city" columns.
2. Rename the aggregated column to reflect the aggregation of the data in the column.
3. Sort the results in ascending order to show the top five retailers along with their region, state, and city that generated the most sales. The final table looks like the following image:

    <img src="https://static.bc-edx.com/ai/ail-v-1-0/m5/lms/img/M5-most-sales-by-retailer.png" alt="image" width="50%" height="50%">

## Determine which Retailer Sold the Most Women's Athletic Footwear
1. Filter the combined DataFrame to create a DataFrame with only women's athletic footwear sales data.
2. Use both the groupby and pivot_table function to create a multi-index DataFrame with the "retailer", "region", "state", and "city" columns.
3. Rename the aggregated column to reflect the aggregation of the data in the column.
4. Sort the results in ascending order to show the top five retailers along with their region, state, and city that sold the most women's athletic footwear. The final table looks like the following image:

    <img src="https://static.bc-edx.com/ai/ail-v-1-0/m5/lms/img/M5-most-womens-footwear-sold-retailer.png" alt="image" width="50%" height="50%">

## Determine the Day and Week with the Most Women's Athletic Footwear Sales
1. Create a pivot table with the "invoice_date" column as the index and the "total_sales" column as the values parameter.
2. Rename the aggregated column to reflect the aggregation of the data in the column.
3. Apply the resample function to the pivot table, place the data into daily bins, and get the total sales for each day.
4. Sort the resampled DataFrame in ascending order to show the top 10 days that generated the most women's athletic footwear sales. The final table, showing the top 10 days looks like the following image:
         
    <img src="https://static.bc-edx.com/ai/ail-v-1-0/m5/lms/img/M5-daily-womens-footwear-sales.png" alt="image" width="25%" height="25%">

5. The final table, showing the top 10 weeks looks like the following image:

    <img src="https://static.bc-edx.com/ai/ail-v-1-0/m5/lms/img/M5-weekly-womens-footwear-sales.png" alt="image" width="25%" height="25%">

## Authored by:
- edX AI Boot Camp - "athletic_sales_analysis_starter_code.jpynb
- Geoff McDaniel - "athletic_sales_analysis_solution_code.jpynb