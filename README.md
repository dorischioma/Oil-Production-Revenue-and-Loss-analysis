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
- Fiscalized production is lower than metered production across all producers, indicating losses that affect revenue. The top producers have fiscalized production significantly lower than metered production. For example, Shell produced 11.2M bbl but only fiscalized 2.0M bbl, indicating a 9.2M bbl loss (~82%).
- Theft volume dropped significantly from 21.15M barrels in 2022 to 5.25M barrels in 2023, representing a 75.16% decrease, indicating improved security or operational measures.
- The long term revenue trend shows that revenue grew steadily from $6bn in 1994 to $46bn in 2011, despite fluctuations. A decline followed, with revenue dropping to $36bn in 2014, and there is a data gap from 2015-2021 (data was not found). After 2021, revenue peaked at $50bn in 2022, but slightly declined to $44bn in 2023, emphasizing the impact of oil price volatility.
- In 2022, Theft/sabotage was the highest contributor to oil loss leading to a loss of (21.15M barrels, 57.63%), followed by measurment error (11.25M barrels, 30.65%). And in 2023 there was a decline, theft/sabotage generated a loss of 5.25M barrels, 64.34% and measurement errors 2.91M, 35.64%, suggesting that theft prevention and accurate metering systems should be prioritized.
--------
### Oil Loss Breakdown by Producers
- **Production and Revenue losses comparison across producers:**
-  In 2022, NNPC 18(formerly Eroton) faces the highest production losses with a 94% overall % loss, it also has the highest discrepancy between metered and fiscalized production, leading to $310.9M loss in revenue, followed closely with the second highest loss is Belema Oil Company, with an 88% overall percentage loss, leading to $124.9M loss in revenue, others are Aiteo Eastern E&P (86%), $155.5M revenue loss and Heirs Energy (62%) with $267.6M loss in revenue. This simply means that this producers lost almost all their production.
- Shell Production Development Company(SPDC) suffered the biggest revenue loss in 2022, despite having a lower percentage loss (32%), SPDC's massive production results in the highest revenue loss of $1.56bn. This suggests that even moderate % losses can lead to significant financial impact. Likewise, NNPC E&P Limited lost $517M which accounts for 13% of its overall production
- Producers like TotalEnergies E&P (29%) and Nigeria Agip Oil Company(25%), experienced relatively lower losses.

### Oil Loss causes
- **Primary causes of Production Losses:** Out of 53 producers, about 21 producers did not record any production loss, the remaining 29 producers have theft accounting for 0ver 90% of total losses in 2022. Producers like NNPC 18 (formerly Eroton) who experienced the highest production loss had theft accounting for 51.9% and measurement error 48% of it's overall loss, while for Belema Oil Company theft accounted for 95.29% of it's loss, For SPDC measurement error led by 43.93%, while theft 36.86%. Moving to 2023, even though there was a decrease in oil loss, theft and measurement error still led in production loss, producers like Heirs Energy, Seplat Energy, Enageed Resources Limited, NOAC and a host of others were badly affected by theft, while producers like Belema Oil Company and Antan Producing Limited were badly affected by measument error. In conclusion, theft is the leading cause of oil loss, followed by measuremnt error and arithmetical errors.
- **Producers with the highest theft volumes**: In 2022 Shell Production Development Company had the highest theft volume (5.6m barrels) which accounts for 36.86% of it's total production, followed closely is NNPC E&P Limited with a theft volume of 2.8m barrels which is 54.91% of it's total production. while it is obvious that this producers have the highest theft volume in terms of numbers, Some other producers lost much more to theft in terms of companies capacity, their theft volume accounts for 65%-99.9% of total production, top 5 producers in this category includes; Seplat Energy (1.8m barrels), NOAC (2.3m barrels), Belema Oil Company (1.18m barrels), Newcross E&P limited (1.1m barrels) and Heirs Energy (1.9m barrels). In 2023 leading the league in terms of numbers is NNPC E&P Limited with a theft volume of 1.2m barrels which is 40.59% of total production, looking at theft volumes with regards to companies capacity, Seplat Energy 1m barrels, accounting to 73.56% of total production, others include NOAC (875k barrels) 80.16% of total production and TotalEnergies (339k barrels) 84.59% of total production. In conclusion, Producers with the highest theft volumes with regards to their company capacity includes; Seplat Energy, NAOC, Belema, Newcross E&P Limited and Heirs Energy.
-------
### Fiscalized Production vs Revenue
 - **Producer with the highest fiscalized production:** TotalEnergies Upstream, Mobil Producing Nigeria Unlimited and Chevron Nigeria Limited had the highest fiscalized production in 2022 and in 2023 Shell Nigeria Exploration Production Company, TotalEnergies Upstream, Mobil Producing Nigeria Unlimited and Chevron Nigeria Limited had the highest fiscalized production.
 - **Fiscalized production and revenue estimates comparison among Producers:** Producers with higher fiscalized production tend to have higher estimated revenue, like TotalEnergies Upstream, Mobil Producing Nigeria Unlimited, and Chevron Nigeria Limited. However, significant discrepancies exist due to production losses, which affects revenue potential. In 2022 NNPC 18 had the largest gap ($310.9M lost revenue), indicating severe losses in fiscalized production. Belema Oil and Aiteo also experience significant revenue losses (above 80% of expected revenue lost). Esso Exploration and Mobil Producing has the smallest revenue gap (>1%), suggesting better production accountability compared to other producers.
- **Relationship between fiscalized production and estimated revenue:** Revenue is directly proportional to fiscalized production, meaning lower fiscalized production leads to lower revenue. NNPC 18, despite producing 3.28M bbl, fiscalized only 205k bbl, leading to a $310.9M revenue loss.
- **Producers with the largest gap between producion and revenue
-------
### Terminal Analysis
- **Terminal operators who own the highest number of crude terminals:** SPDC (Shell Petroleum Development Company) operates the most crude terminals (15 terminals).
- **Terminal operators with the highest error rates in production records:** SPDC shows the highest error rates (98.23%) 
- **Crude Terminals at the highest risk of oil theft:** Bonny terminal is the most vulnerable to theft (56.64%), followed by Forcados (23.5%), Brass (15%.5), Bonny (OML 11) and Escravos.
- **How production vary across crude terminals:** MPN and SPDC terminals have the highest fiscalized production volumes.
