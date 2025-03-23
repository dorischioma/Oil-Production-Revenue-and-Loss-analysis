# Oil-Production-Revenue-and-Theft-analysis

## Project Overview:
Oil production and revenue are major issues, and theft (like pipeline vandalism) is a huge challenge that affects national income. 
This project aims to analyze how oil theft impacts production and revenue and to identify trends and patterns in oil theft incident.
This project involves finance, economics, security and operations data.
By leveraging diagnostic and predictive analysis, this project will show how theft patterns correlate with revenue drops or production shortages.
Key stakeholders include oil companies, government and investors.

## Key Questions:
- What is the overall production loss by year.
- Which Producer had the highest revenue loss?
- What factors contributes the most to oil loss?
- Which Producer has the highest percentage loss?
- What is the relationship between between fizcalized production and fiscalized revenue, does theft have any impact?
- Who owns the highest crude terminal
- Which crude terminals is high risk for theft, error and other oil loss
- Which crude terminals is Safe from theft ?
- Which crude terminal is the safest from thefft
- Who produces the most oil
- which terminal operator has the higest operationall loss

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

