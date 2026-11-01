**CAPSTONE 2: CLEANING MESSY SALES DATA WITH SQL**

**1. Project Overview**

This project examines the data-cleaning and analysis of a café sales dataset using SQL and SQLite. The work covers data inspection, identification of data-quality issues, cleaning and validation, and the use of SQL queries to produce meaningful sales summaries.
The analysis examines product performance and sales across service channels, providing a structured view of the available transaction data.

**2. Project Objectives**

Assess the structure and quality of the café sales dataset.
Identify and document missing, inconsistent, and invalid data.
Apply appropriate cleaning and validation procedures.
Use SQL queries to analyse sales and transaction patterns.
Present the findings through summary tables and visualisations.

**3. Tools and Technologies**

SQLite and SQL — data staging, inspection, cleaning, validation, and analysis.
Jupyter Notebook — development and documentation of the analytical workflow.
Python — supporting data preparation and visualisation.
Microsoft Excel and Power BI — presentation and reporting of the prepared results.

**4. Project Structure**

data/ — cleaned café sales dataset.
notebooks/ — notebook documenting the data preparation, SQL queries, validation, and analysis.
docs/ — supporting issue register, process report, validation report, and prompt reflection log.
reports/visuals/ — charts presenting the sales analysis.
PowerBI_Ready_Cafe_Sales.xlsx — cleaned transaction data and supporting summary tables.
Cafe_Sales_Interactive_Dashboard.html — interactive presentation of the key findings.

**5. Dataset and Data Quality Assessment**

The dataset contains café sales transaction records, including transaction identifiers, items, quantities, unit prices, total amounts, payment methods, service channels, and transaction dates.
The data-quality assessment identified missing values in Item (969 records; 9.69%), Payment Method (3,178 records; 31.78%), Location (3,961 records; 39.61%), and Transaction Date (460 records; 4.60%). These gaps were considered during the interpretation of the analysis to avoid treating unknown information as confirmed values.
The Location field contains the categories In-store and Takeaway. These categories represent service channels rather than geographical regions. Although Drive-thru appeared in a reference list, it was not present in the observed transaction records. Consequently, the dataset does not support a geographical or regional sales comparison.
The source dataset does not specify a currency. Monetary results are therefore reported as numeric values without assigning a currency symbol.

**6. Analytical Approach**

The analysis followed a structured workflow. The source data was loaded into a staging table and examined to understand its fields, data types, category distributions, and completeness. Data-quality issues were recorded and addressed through the cleaning process.
SQL queries were then used to validate the prepared data and aggregate sales by product and service channel. The resulting summaries were used to identify leading products, compare recorded sales across service channels, and examine transaction patterns. Visualisations were prepared to communicate the main results.

**7. Findings and Results**

The cleaned dataset contains 9,960 records with a valid Total Spent value, representing recorded sales of 88,952.00. The average value per valid sales record is 8.93. These figures describe the transactions with a recorded sales amount and should be interpreted in the context of the dataset's identified data-quality limitations.
Product-level analysis shows that Salad generated the highest recorded sales, totalling 17,320.00. Sandwich followed with 13,664.00, while Smoothie generated 13,320.00. Combined, these three products contributed approximately 55.1% of recorded sales for transactions with a known product. Coffee recorded the highest transaction count, with 1,165 transactions.
Service-channel analysis recorded sales of 27,127.00 across 3,017 In-store transactions and 26,487.50 across 3,022 Takeaway transactions. A further 35,337.50 in recorded sales was associated with transactions where the service-channel value was missing. The missing service-channel information is substantial and limits the completeness of the comparison between In-store and Takeaway activity.
Overall, the results indicate that Salad was the leading product by recorded sales, while Coffee had the highest transaction frequency. Recorded sales across the two identified service channels were similar; however, the volume of sales associated with missing channel information means that the channel comparison should be interpreted with caution.

**8. Limitations**

Missing values in product, payment method, service channel, and transaction date fields limit the completeness of some analyses.
The Location field identifies service channels rather than geographical locations; therefore, regional performance cannot be assessed from this dataset.
The source data does not identify the currency used for the monetary values.
The findings describe patterns in the available records and do not establish the causes of customer purchasing behaviour.

**9. Project Deliverables**

The completed project includes the SQL/Jupyter Notebook, cleaned café sales dataset, data-quality issue register, process report, validation report, prompt reflection log, sales visualisations, Power BI-ready Excel workbook, and interactive HTML dashboard.

**10. Conclusion**

This project applied a structured SQL-based approach to cleaning and analysing café sales data. The process identified important data-quality limitations, produced a validated dataset for analysis, and generated sales summaries that highlight product performance and service-channel activity. The findings provide a useful overview of the available sales records while recognising the limitations created by missing information and the absence of geographical and currency details.

