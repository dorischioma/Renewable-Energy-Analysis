# Renewable-Energy-Analysis

## INTRODUCTION
For decades, global energy demand was met primarily by fossil fuels (coal, oil, and natural gas). While these sources powered industries and economies, they also contributed significantly to greenhouse gas emissions, air pollution, and environmental degradation.
As the impact of climate change became more evident, the need for cleaner, more sustainable energy alternatives grew urgent. This gave rise to renewable energy, energy derived from natural processes that are constantly replenished, such as sunlight, wind, water, and geothermal heat.
Renewable energy is not just an alternative; it is a transformative solution at the heart of the global transition toward sustainability. 
The key conclusions, methodology for the analysis and recommendations resulting from analyzing the renewable energy dataset for Great Britain and Germany are covered in the sections that follow. 

## OVERVIEW
In this project, we set out to answer key questions about the energy markets in Germany (DE) and Great Britain (GB). Our main focus was on comparing wholesale electricity prices, understanding trends in forecasted capture prices for solar and wind technologies, and exploring how power generation influences pricing.

## DATA SOURCE:
[File: Energy market analysis_Clean file]
•	Wholesale Price
•	Capture Price
•	Generation Mix
•	Processed Summary
•	Technology Table
•	Geography Table


## TOOLS USED:
•	Microsoft Excel (data cleaning)
•	Power BI (visualization & analysis)

## DATA CLEANING:
To prepare the data, we used Power Query in Excel to:
•	Structure the table.
•	Transpose the columns
•	Rename columns for clarity
•	Change data types (prices, GWh)
We also created lookup tables in excel to merge datasets by common fields like geography and Technology.

## KEY QUESTIONS & FINDINGS
1.	How do wholesale power prices (baseload) compare between GB and DE and whether their respective power generation mix could explain the difference?

Between 2023-2050, Baseload prices in Great Britain are consistently lower compared to Germany, and their power generation mix differs significantly. 


Germany’s higher Baseload price is attributed to her heavy reliance on Onshore Wind and Solar PV, which are intermittent energy sources, when wind and solar production are low, Germany may need to rely more on expensive backup sources like gas, thereby driving baseload prices higher compared to GB.
 
 While Great Britain leans more on Offshore Wind and Nuclear, both of which provide more stable output. Nuclear provides steady baseload, and offshore is generally stronger and more consistent than onshore wind. This stability helps keep GB’s baseload prices lower.
 




2.	From a capture price perspective, which technology offers better potential between solar PV in GB and onshore wind in DE? 
Between 2023 to 2050, Solar PV in GB shows an average capture price of €66.58, while Onshore Wind in DE averages €75.14.  However, a lower capture price indicates better market alignment, a more affordable or stable returns and can be more attractive from a commercial perspective. This suggests that Solar PV in GB will offer better long-term revenue potential, depending on factors like volume or policy.

 

3.	In the long run, is there a relationship between capture prices and power generation output (GWh) for solar PV and onshore wind in DE? 
The scatter chart below illustrates the long-run relationship between capture prices and power generation output for Solar PV and Onshore Wind in Germany (DE). The analysis shows that Onshore Wind consistently has both a higher average capture price and greater total generation output compared to Solar PV. This indicates a positive relationship between the two variables, technologies with higher capture prices tend to have higher generation outputs. The trend suggests that Onshore Wind offers stronger potential for long-term generation capacity, possibly due to more favorable wind conditions or more mature infrastructure in Germany.

 



4.	Did Aaron change his forecast for solar PV and onshore wind capture prices between Q3 2022 and Q1 2023? If so, how significant is the shift and what could possibly explain that? (Some Internet search might be needed for this part.) 
Aaron changed his forecast for solar PV and onshore wind capture prices between Q3 2022 and Q1 2023. For example, the capture price for solar PV in GB for 2025 was revised from €94/MWh in Q3 2022 to €130/MWh in Q1 2023, representing a 38.72% change.

 
This change was driven by the economic attractiveness of PV, advancement in supply chains and supportive policies.

CONCLUSION
1.	Wholesale Price and Generation Mix Discrepancy:
The baseload price comparison reveals that Germany often reports higher wholesale prices than Great Britain. This could be partially explained by Germany's heavier reliance on renewables, supported by a more diversified generation mix, including strong solar and wind penetration.
2.	Technology Comparison Insight:
When comparing solar PV in GB and onshore wind in DE, solar PV exhibits a stronger and more stable upward trend in capture prices. This trend indicates greater revenue potential and market alignment for solar PV in GB in the near to medium term.
3.	Capture Price vs Generation Output in DE:
While both solar PV and onshore wind in DE show general growth in generation over time, the correlation with capture prices is not linear. This suggests that simply expanding capacity does not always equate to higher economic returns.
4.	Forecast Adjustment Insight:
Aaron’s forecast between Q3 2022 and Q1 2023 shows a notable upward revision in both solar PV and onshore wind capture prices. This is attributed to its cost competitiveness, economic attractiveness of PV and massive deployment of supply-chain

RECOMMENDATIONS
1.	Monitor Policy and Market Sentiment
Continue monitoring changes in government policy (e.g., subsidies, tax incentives) and market signals that could affect capture prices, especially in light of geopolitical or economic shifts. These have proven to be major contributors to forecast adjustments.
2.	Strategic Focus on Solar PV in GB
Given the stronger price growth trend, GB’s solar PV may offer better investment potential. Stakeholders may want to prioritize this segment in terms of project development, funding, or policy advocacy.
3.	Balance Expansion with Market Conditions
While increasing renewable generation is key to sustainability, producers and regulators should monitor how additional capacity impacts capture prices. Overcapacity without proportional demand growth could depress prices, reducing project profitability.
