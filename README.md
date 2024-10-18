#Marketing Analytics Report: US Stroller Market
This project contains an RMarkdown (.RMD) file that generates a report on the US stroller market using sales data and the Bass Diffusion Model for marketing analytics.

#Author
#Hovik Voskanyan

#Date
2024-10-17

Overview
The purpose of this analysis is to examine the US stroller market based on sales data and apply the Bass diffusion model to estimate market potential, innovation, and imitation coefficients. The report is generated in PDF format.

#Files and Directories
1. report/
MarketingAnalytics.Rmd: The main RMarkdown file that generates the marketing analytics report in PDF format.
2. data/
StrollerSalesData.xlsx: The sales data for the US stroller market, used in the analysis.
Setup
Required Libraries
Before running the RMarkdown file, ensure you have the following R packages installed:

r
Copy code
install.packages(c("ggplot2", "ggpubr", "knitr", "readxl", "diffusion"))
Running the Report
Clone the repository and ensure that the directory structure remains the same (data folder for the Excel file, report folder for the RMD file).
Open MarketingAnalytics.Rmd in RStudio or any RMarkdown editor.
Ensure the StrollerSalesData.xlsx file is located in the data/ folder.
Render the report by clicking the "Knit" button in RStudio, or run the following R code:
r
Copy code
rmarkdown::render("report/MarketingAnalytics.Rmd")
This will generate a PDF report analyzing the US stroller market based on the provided data.

Data
StrollerSalesData.xlsx: This file contains the yearly sales data for the US stroller market.
The sales data is multiplied by 1,000,000 to reflect the actual units sold.
Analysis
The analysis includes:

Visualization of yearly sales data.
Estimation of the Bass diffusion model parameters (p, q, and M).
Comparison of predicted vs actual sales peaks.
Application of the diffusion package to calculate market potential and parameters.
Results
The report will provide:

A bar chart of yearly stroller sales.
Bass model parameter estimates (p, q, and M).
Diffusion curve based on the estimated parameters.

References:
Data is taken from : https://www.statista.com/statistics/633336/retail-sales-value-of-the-north-american-stroller-market/