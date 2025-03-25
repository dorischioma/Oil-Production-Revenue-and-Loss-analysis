# Oil-Production-Revenue-and-Theft-analysis

## Project Overview:
Oil production and revenue are major issues, and theft (like pipeline vandalism) is a huge challenge that affects national income. 
This project aims to analyze how oil theft impacts production and revenue and to identify trends and patterns in oil theft incident.
This project involves finance, economics, security and operations data.
By leveraging descriptive and diagnostic analysis, this project will show how theft patterns correlate with revenue drops or production shortages.
Key stakeholders include oil companies, government and investors.

## Problem Statement:
Oil theft and pipeline vandalism have led to significant production losses, reduced fiscalized revenue, and increased security risks in the oil and gas industry. This issue affects national income and threatens economic stability. Despite existing measures, theft patterns continue to evolve making it critical to analyze their impact on production and revenue to develop effective mitigation strategies.

## Key Questions:
- What is the overall production loss by year.
- Who produces the most oil
- Which Producer experienced the highest revenue loss due to oil theft and operational losses?
- Which Producer has the highest percentage loss?
- Who owns the largest crude terminal
- Which terminal operator has the highest operational loss
- What is the relationship between between fizcalized production and fiscalized revenue, does theft have any impact?
- What factors contributes the most to oil loss?
- Which crude terminlas are at the highest risk for theft, operational errors or other losses?
- What are the key factors that make certain crude terminals more vulnerable to theft and operational losses?
- Which crude terminal is the safest from theft
  
## Data Sources:
-	NEITI
-	EIA

## Tools
- Excel
- Power BI

### Data cleaning
1.	Handling Theft/Sabotage data:
The theft/sabotage column in the crude oil production 2022-2023 dataset represents the volume of crude oil lost due to theft, sabotage or vandalism. This information is crucial for understanding production losses and their impact on fiscalized production and revenue. However, during data review, I observed that no theft values were recorded for the year 2022, all fields under this column were either blank or missing. Additionally for years, theft values are expected to be all negative, as negative values would not make logical sense in this context. Using power query in excel,
-	I replaced missing values in theft sabotage for 2022 with zero, assuming that there was no reported theft in 2022.
-	Negative values in Theft/sabotage were replaced with zero as theft losses cannot be negative.
2.	Ensuring accuracy and consistency:
Historical production and revenue data was downloaded precleaned and organized already, brent raw data also came in clean, but for the purpose of this analysis, I had to aggregate the price for each year, meanwhile, for the crude production 2022-2023 data I had to remove unnecessary columns, handle duplicates and missing values, restructure the data into a more suitable format for analysis, additionally, I standardized the dataset by ensuring consistency in text formatting. 


## Key Insights
### Production Loss and Revenue Trend by Year
- Production Loss by year: 2023 saw a significant reduction (7.68M barrels) compared to 2022 (36.69M barrels) indicating improved security or operational measures.
- Factors contributing to loss: Theft and measurement errors are the biggest contributors, accounting for 91% of total losses.
- Total Revenue trend: Revenue grew steadily from $6bn in 1994 to $46bn in 2011, despite fluctuations. A decline followed, with revenue dropping to $36bn in 2014, and there is a data gap from 2015-2021. After 2021, revenue peaked at $50bn in 2023, but slightly declined to $44bn in 2023.


