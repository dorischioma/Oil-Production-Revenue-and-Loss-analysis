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
- How has oil production changed between 2022 and 2023?
- How has fiscalized production changed, and what does this mean for revenue?
- How much oil was lost to theft in 2023 compared to 2022?
- How has total revenue trended from 1994 to 2024?
- Which oil companies experience the highest losses in production?
- How do revenue losses compare across different producers?
- What are the primary causes of production losses?
- Which companies have the highest theft losses?
- Which oil producers have the highest fiscalized production?
- How do fiscalized production and revenue estimates compare among producers?
- What is the relationship between fiscalized production and estimated revenue?
- Which producers have the largest gaps between production and revenue?
- Which terminal operators own the highest number of crude terminals?
- Which terminal operators have the highest error rates in production records?
- Which terminals are at the highest risk of oil theft?
- How does production vary across different crude terminals?

  
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
- In 2023 Metered Production increased by 3.34% (545.25M barrels), compared to 2022 (527.64M barrels) while in 2023 fiscalized production saw a 9.5% increase (537.57M barrels), compared to 2022 (490.94M barrels), indicating better efficiency.
- Theft volume dropped significantly from 21.15M barrels in 2022 to 5.25M barrels in 2023, representing a 75.16% decrease, indicating improved security or operational measures.
- The long term revenue trend shows that revenue grew steadily from $6bn in 1994 to $46bn in 2011, despite fluctuations. A decline followed, with revenue dropping to $36bn in 2014, and there is a data gap from 2015-2021 (data was not found). After 2021, revenue peaked at $50bn in 2022, but slightly declined to $44bn in 2023, emphasizing the impact of oil price volatility.
- In 2022, Theft/sabotage was the highest contributor to oil loss leading to a loss of (21.15M barrels, 57.63%), followed by measurment error (11.25M barrels, 30.65%). And in 2023 there was a decline, theft/sabotage generated a loss of 5.25M barrels, 64.34% and measurement errors 2.91M, 35.64%, suggesting that theft prevention and accurate metering systems should be prioritized.

### Oil Loss Breakdown by Producers
- NNPC 18(formerly Eroton) faces the highest losses (94% loss rate), but it's revenue loss is $0.31M which is lower than Shell Production and Development Company 
- Shell, NNPC E&P, and Nigerian Agip lost the most revenue.

