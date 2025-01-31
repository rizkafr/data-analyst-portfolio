# Coffee Sales Report (Interactive Dashboard creation using MS Excel)

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset used](#dataset-used)
- [Questions (KPIs)](#questions-kpis)
- [Process](#process)
- [Dashboard](#dashboard)
- [Conclusion](#conclusion)
- [Key Takeaways](#key-takeaways)
- [Future Enhancements](#future-enhancements)

## Project Overview
This project involves creating an Excel dashboard to analyze coffee sales data. The dashboard will include visualizations of sales volume, total revenue, sales trends over time, sales distribution by country, and top-performing customers. Advanced Excel features like slicers, filters, timeline tools, pivot tables, XLOOKUP, and INDEX MATCH will be utilized to create an interactive and comprehensive analysis.

## Dataset used
- <a href="https://github.com/rizkafr/data-analyst-portfolio/blob/main/coffee-sales-report/Coffee%20Sales%20Report_Data.xlsx">Dataset</a>

## Questions (KPIs)
- How many kilograms of coffee were sold during the specified period?
- What is the total revenue generated from coffee sales?
- What are the sales trends over time?
- How are coffee sales distributed across different countries?
- Who are the top 5 customers making the most purchases?
- How do different roast types, sizes, loyalty card usage, and time periods influence the sales volume, total revenue, sales trends, sales distribution, and top customers?


## Process
1. **Data Preparation**:
   - Import the provided Excel data into the workbook.
   - Use Excel functions to clean and preprocess the data, such as removing duplicates, handling missing values, and standardizing formats.
   - Convert the orders sheet into a table to facilitate easy updates and refreshing of pivot tables.

2. **Data Integration**:
   - Use XLOOKUP and INDEX MATCH functions on the orders sheet to retrieve data from the customers and products sheets.
     - Example of XLOOKUP formula:
       ```excel
       =XLOOKUP(C2;customers!$A$1:$A$1001;customers!$B$1:$B$1001;;0)
       ```
       **Note**: The XLOOKUP formula is not available in older versions of Excel. To use this formula, consider using Excel for Microsoft 365 or Excel Online.
     - Example of INDEX MATCH formula:
       ```excel
       =INDEX(products!$A$1:$G$49;MATCH(orders!$D2;products!$A$1:$A$49;0);MATCH(orders!I$1;products!$A$1:$G$1;0))
       ```

3. **Data Analysis**:
   - Use pivot tables to summarize and analyze the data.
   - Calculate key metrics such as total sales, total revenue, and sales trends over time.

4. **Dashboard Design**:
   - Create a new Excel sheet for the dashboard.
   - Design the layout of the dashboard, including charts, and key metrics.
   - Use Excel features like slicers, filters, and timeline tools to make the dashboard interactive.

5. **Visualization**:
   - Create visualizations such as bar charts and line graphs to represent the data.
   - Ensure visualizations are clear, informative, and easy to understand.

6. **Dynamic Analysis**:
   - Incorporate slicers and filters to allow users to interact with the data based on roast types, sizes, loyalty card usage, and time periods.
   - Ensure the dashboard updates dynamically based on user selections.

7. **Review and Testing**:
   - Review the dashboard for accuracy and completeness.
   - Test the dashboard to ensure all interactive elements work as expected.
   - Make any necessary adjustments based on feedback.

8. **Deployment**:
   - Save the final version of the dashboard.
   - Share the dashboard via OneDrive and GitHub for easy access and collaboration.

## Dashboard

![Screenshot Dashboard](https://github.com/rizkafr/data-analyst-portfolio/blob/main/coffee-sales-report/Coffee%20Sales%20Report_Dashboard.jpg)

You can view the interactive Coffee Sales Dashboard by clicking [here](https://github.com/rizkafr/data-analyst-portfolio/blob/main/coffee-sales-report/Coffee%20Sales%20Report_Dashboard.xlsx). For a seamless experience without downloading, you can also access the dashboard on OneDrive [here](https://1drv.ms/x/c/34170c969df0cedc/EQtRyq5oj3pKtqEq1frFmfoBI7usvPowi6SsUSXAW9aOjg?e=wDeyId).

## Conclusion

The Coffee Sales Dashboard project demonstrates the power of data visualization in transforming raw data into actionable insights. By leveraging interactive elements such as slicers, filters, and timeline tools, the dashboard provides a comprehensive view of coffee sales, enabling stakeholders to make informed decisions.

### Key Takeaways
- **Interactive Visualizations**: The dashboard allows users to explore data dynamically, providing a deeper understanding of sales trends, customer behavior, and geographical distribution.
- **Data-Driven Decisions**: Visualizing key metrics such as total sales, revenue, and top customers helps identify opportunities for growth and areas for improvement.
- **User-Friendly Interface**: The intuitive design of the dashboard ensures that users can easily navigate and interact with the data, making it accessible to both technical and non-technical stakeholders.

### Future Enhancements
- **Advanced Analytics**: Incorporating advanced analytics techniques such as predictive modeling and machine learning to further enhance the insights provided by the dashboard.
- **Real-Time Data**: Integrating real-time data sources to provide up-to-date information and enable more timely decision-making.
- **Expanded Metrics**: Adding additional metrics and visualizations to cover other aspects of the business, such as inventory management and customer satisfaction.

By focusing on data visualization, this project highlights the importance of presenting data in a clear and engaging manner to drive better business outcomes.

