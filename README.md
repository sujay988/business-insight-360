
## Business Insights 360

## Project Overview

Project Overview:
AtliQ Hardware is experiencing significant growth, prompting the decision to adopt data analytics using Power BI for the first time. This strategic move aims to outpace competitors and foster data-driven decision-making within the company. The project endeavors to address stakeholder inquiries across finance, sales, marketing, and supply chain domains.

This initiative was undertaken following the Codebasics Power BI Course, which provided invaluable guidance and insights.
My Power Bi  dashboard [Here live report link](https://app.powerbi.com/links/JhM76t8BQA?ctid=c6e549b3-5f45-4032-aae9-d4244dc5b2c4&pbi_source=linkShare&bookmarkGuid=484d52fb-5a7e-48ef-a436-f8d926e098c0)

## Tech stacks
- SQL
- PowerBi Desktop
- Excel
- DAX language
- DAX studio (for optimizing the report)
- Project charter file

## PowerBI techniques Learnt
- what are all the questions should be asked before staring the project
- Creating calculated columns
- creating measure using DAX language
- Data modeling
- Using Bookmarks to switch between two visuals
- Page navigation with buttons
- Using divide function to prevent zero division errors
- creating date table using m language
- Dynamic titles based on the applied filters
- Using KPI indicators
- Conditional formatting the values in visuals using icons or background color
- Data validation techniques
- PowerBi services
- Publishing reports to PowerBi services
- Setting up personal gateway to set up the auto refresh of data
- PowerBi App creation
- Collaboration, workspace, access permissions in PowerBi services

## Business related terms
- Gross price
- Pre-invoice deductions
- Post-Invoice deductions
- Net Invoice sale
- Gross Margin
- Net sales
- Net profit
- COGC - cost of goods sold
- YTD - Year to Date
- YTG - Year to Go
- Direct
- Retailer
- Distributors
- Consumer


## AltiQ Hardware: Building an Analytics Team for Data-Driven Success

AltiQ Hardware, a rapidly expanding global enterprise specializing in computer and accessories sales, has recently encountered unforeseen setbacks with its venture into the American market. Despite leveraging surveys, intuition, and rudimentary Excel analysis, the company faced unexpected losses. Moreover, the presence of formidable competitors equipped with robust analytics teams underscores the urgent need for AltiQ Hardware to establish its own analytics team.

## Project Kickoff Session: Clarifying Objectives and Expectations

Before diving into dashboard development, it's imperative to address critical questions:

1. **Objective:** What is the primary goal of this Power BI dashboard?
2. **Success Metrics:** How will we measure the success of this project?
3. **Timeline:** What is the project deadline?
4. **Preview Expectations:** Do stakeholders expect a preview before the official release?
5. **Stakeholder Expectations:** What are the stakeholders' hopes and fears regarding this project?
6. **Dashboard Users:** Who will use the dashboard and for what purposes?
7. **Completion Expectations:** What outcomes do stakeholders anticipate upon project completion?
8. **Potential Challenges:** What are the potential obstacles in building this dashboard?
9. **Required Resources:** What data and resources are needed to build this dashboard?
10. **Stakeholder Inputs:** Do stakeholders have any design or view preferences for the dashboard?


## Exploring the Dataset: Understanding Available Data

Understanding what data is available will be more helpful while doing analysis. before jumping on to the analysis get good understanding of what are data available.

Dimension table : It will have the static data like details of customer and products
Fact table : It will have the data about the transactions

- gdb041:
  - dim_customer
    - 27 distinct markets (ex India, USA, spain)
    - 75 distinct customers thorough out the market
    - 2 types of platforms
      - Brick & Motors - Physical/offline store
      - E-commerce - Online Store (Amazon, flipkart)
    - Three channels
      - Retailer
      - Direct
      - Distributors
   - dim_market
     - 27 distinct markets (ex India, USA, spain)
     - 7 sub-zones
     - 4 regions
       - APAC
       - EU
       - nan
       - LATAM
    - dim_product
      - Divisions
        - P & A
          - Peripherals
          - Accessories
        - PC
          - Notebook
          - Desktop
        - N & S
          - Networking
          - Storage
      - There are 14 different categories, Like Internal HDD, keyboard
      - There are different variants available for the same product
   - fact_forecast_monthly
     - This table is used to forecast the customer’s need in advance, which can help in
       - Higher customer satisfaction
       - Reduced cost in warehouses for storage purpose
     - The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
     - All the date of the month will be replaced by the start date of the month
     - It will have all the column names and in the end it will have the forecast quantity need of the customer
   - fact_sales_monthly
     - his table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.
- gdb056
    - freight_cost
      - This table has details of travel cost and other cost for each market with fiscal year
    - gross_price
      - as the details of gross prices with product code
    - manufacturing_cost
      - Has the details of manufacturing cost with product code with year
    - Pre_invoice_dedutions
      - as the details of pre invoice deductions percentage for each cutomer with year
    - Post_invoice_deductions
      - Post invoice deductions and other deductions details

## Importing data into PowerBi
- As the database is MySQL in this project, we need to import the datasets from Mysql database to PowerBi by providing the Database access credential

## Data Model
- Data modeling plays a vital role and is considered as the basement of report. All the visuals will be build upon the data model.
- Poor data modeling affects the over all performance of the report.
- Following Good practices of data modeling is must. Refer this page to get to know the good practices Blog
- In this project, we have followed Snowfall data modeling method.



## Dashboard designing
Based on the mock ups received as requirement, the team will start designing the visuals and create measure as and when required

## Home view
In Home view, all the views button will be available. User will land on specific view page by clicking the button

- Home
- Finance View
- Sales View
- Marketing View
- Supply chain View
- Executive View




you can find the full report file here : [Here live report link](https://app.powerbi.com/links/JhM76t8BQA?ctid=c6e549b3-5f45-4032-aae9-d4244dc5b2c4&pbi_source=linkShare&bookmarkGuid=484d52fb-5a7e-48ef-a436-f8d926e098c0)


## Project Outcome
By using this report, decisions can be taken based on the data. Further it will help in answering n number of why questions based on the situations.
