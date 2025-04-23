# Power Market Forecast Analysis for Strategic Planning (GE & DE, 2023-2050)

## INTRODUCTION
This Project Supports Laura, a strategic planning director at a European renewable energy firm, in analyzing power market forecasts for Great Britain (GB) and Germany (DE). With her analysts temporarily unavailable, Laura needs to independently interpret forecast data, identify trends and differences, and make informed planning decisions using a dynamic Power Bi dashboard.

## OVERVIEW
The analysis focuses on comparing power generation and pricing trends in GB and DE for the 2023–2050 period. Specifically, it evaluates wholesale prices, capture prices, and generation forecasts for solar PV and onshore wind technologies. Additionally, the project aims to build a sustainable solution that allows automated data updates and user-driven insights through a self-service Power BI dashboard.

## DATA SOURCE
[Excel spreadsheets shared via Dropbox by two analysts (Aaron for GB, Brian for DE)](https://github.com/dorischioma/Renewable-Energy-Analysis/blob/main/Energy%20market%20analysis_%20Raw%20file.xlsx/)  
Each spreadsheet includes:
- Forecasts from Q3 2022 and Q1 2023
- Variables: Generation Capacity (MW), Power Generation (GWh), Wholesale Price (€/MWh), Capture Price (€/MWh)
- Forecast horizon: 2022–2050
- Technologies: Solar PV, Onshore Wind



## TOOLS USED:
- Microsoft Excel: Initial data inspection, cleaning, and structuring
-	Power Query (in Excel): Data transformation and ETL
- Power BI – Interactive dashboard design and visual analysis

## DATA CLEANING:
I took the follwing steps to prepare the data:
- **Consolidated multiple Excel files**: I had multiple Excel files from two people (Aaron and Brian), each with data for different countries and quarters. I combined them into one table so everything was in one place and easier to work with.
- **Unpivoted the table layout**: The original Excel files had years (2022–2060) as column headers, which makes it hard to analyze. I changed the format so each row shows one value for one year.
- **Adding Extra Columns**: We created new columns to describe each row better — like which country it belongs to, the type of technology (solar or wind), and whether it came from the Q3 2022 or Q1 2023 file. These labels help us compare and analyze the data easily. 
- **Applying Currency and Inflation Adjustments**:
Since i was comparing prices across countries and years, i used the provided exchange rates (GBP to EUR) and inflation rates to adjust prices. This helped me make fair comparisons, especially between different time periods.
The cleaned Excel file is [here](https://github.com/dorischioma/Renewable-Energy-Analysis/blob/main/Energy%20market%20analysis_Cleaned%20file.xlsx/)

## KEY BUSINESS QUESTIONS & INSIGHTS
### 1.	How do wholesale power prices (baseload) compare between GB and DE and whether their respective power generation mix could explain the difference?
**Insights**
  Between 2023-2050, Baseload prices in Great Britain are consistently lower compared to Germany, and their power generation mix differs significantly. 
[Wholesale Prices Comparison](https://github.com/dorischioma/Renewable-Energy-Analysis/blob/main/Baseload%20comparison%20screenshot.png/)

  Germany’s higher Baseload price is attributed to her heavy reliance on Onshore Wind and Solar PV, which are intermittent energy sources, when wind and solar production are low, Germany 
  may need to rely more on expensive backup sources like gas, thereby driving baseload prices higher compared to GB.
  [DE power generation mix](https://github.com/dorischioma/Renewable-Energy-Analysis/blob/main/DE%20Generation%20Mix.png/)
 
  While Great Britain leans more on Offshore Wind and Nuclear, both of which provide more stable output. Nuclear provides steady baseload, and offshore is generally stronger and more 
  consistent than onshore wind. This stability helps keep GB’s baseload prices lower.
  [GB power generation mix](https://github.com/dorischioma/Renewable-Energy-Analysis/blob/main/GB%20Power%20Generation%20Mix.png/) 


### 2.	From a capture price perspective, which technology offers better potential between solar PV in GB and onshore wind in DE?**
**Insight**
Between 2023 to 2050, Solar PV in GB shows an average capture price of €66.58, while Onshore Wind in DE averages €75.14.  However, a lower capture price indicates better market alignment, a more affordable or stable returns and can be more attractive from a commercial perspective. This suggests that Solar PV in GB will offer better long-term revenue potential, depending on factors like volume or policy.
[Capture price comparison by technology](https://github.com/dorischioma/Renewable-Energy-Analysis/blob/main/Avg%20Capture%20Price%20by%20technology%20screenshot.png/)
 

### 3.	In the long run, is there a relationship between capture prices and power generation output (GWh) for solar PV and onshore wind in DE?
**Insight**
The scatter chart below illustrates the long-run relationship between capture prices and power generation output for Solar PV and Onshore Wind in Germany (DE). The analysis shows that Onshore Wind consistently has both a higher average capture price and greater total generation output compared to Solar PV. This indicates a positive relationship between the two variables, technologies with higher capture prices tend to have higher generation outputs. The trend suggests that Onshore Wind offers stronger potential for long-term generation capacity, possibly due to more favorable wind conditions or more mature infrastructure in Germany.
[Relationship between capture price & power generation](https://github.com/dorischioma/Renewable-Energy-Analysis/blob/main/Relationship%20between%20capture%20price%20%26%20power%20generation%20in%20DE%20screenshot.png)

### 4.	Did Aaron change his forecast for solar PV and onshore wind capture prices between Q3 2022 and Q1 2023? If so, how significant is the shift and what could possibly explain that?(Some Internet search might be needed for this part.) 
**Insight**
Aaron changed his forecast for solar PV and onshore wind capture prices between Q3 2022 and Q1 2023. For example, the capture price for solar PV in GB for 2025 was revised from €94/MWh in Q3 2022 to €130/MWh in Q1 2023, representing a 38.72% change.
[Aaron's Forecast change](https://github.com/dorischioma/Renewable-Energy-Analysis/blob/main/Forecast%20comparison%20in%20GB%20screenshot.png/)

This change was driven by the economic attractiveness of PV, advancement in supply chains and supportive policies.

## DASHBOARD
[Dashboard](https://github.com/dorischioma/Renewable-Energy-Analysis/blob/main/Dashboard.png/)

## CONCLUSION
1.	Wholesale Price and Generation Mix Discrepancy:
The baseload price comparison reveals that Germany often reports higher wholesale prices than Great Britain. This could be partially explained by Germany's heavier reliance on renewables, supported by a more diversified generation mix, including strong solar and wind penetration.
2.	Technology Comparison Insight:
When comparing solar PV in GB and onshore wind in DE, solar PV exhibits a stronger and more stable upward trend in capture prices. This trend indicates greater revenue potential and market alignment for solar PV in GB in the near to medium term.
3.	Capture Price vs Generation Output in DE:
While both solar PV and onshore wind in DE show general growth in generation over time, the correlation with capture prices is not linear. This suggests that simply expanding capacity does not always equate to higher economic returns.
4.	Forecast Adjustment Insight:
Aaron’s forecast between Q3 2022 and Q1 2023 shows a notable upward revision in both solar PV and onshore wind capture prices. This is attributed to its cost competitiveness, economic attractiveness of PV and massive deployment of supply-chain

## RECOMMENDATIONS
1.	Monitor Policy and Market Sentiment
Continue monitoring changes in government policy (e.g., subsidies, tax incentives) and market signals that could affect capture prices, especially in light of geopolitical or economic shifts. These have proven to be major contributors to forecast adjustments.
2.	Strategic Focus on Solar PV in GB
Given the stronger price growth trend, GB’s solar PV may offer better investment potential. Stakeholders may want to prioritize this segment in terms of project development, funding, or policy advocacy.
3.	Balance Expansion with Market Conditions
While increasing renewable generation is key to sustainability, producers and regulators should monitor how additional capacity impacts capture prices. Overcapacity without proportional demand growth could depress prices, reducing project profitability.

## TRAINING GUIDE  
To carry out this analysis, the training guide is found [here](https://github.com/dorischioma/Renewable-Energy-Analysis/blob/main/Training_Guide.docx/)
