# Railway Travel Company 

![Railway logo](https://github.com/user-attachments/assets/4bec1009-7af5-4806-89a8-6f9b5d92cfe6)

## Table of Contents
- [EXECUTIVE SUMMARY](#executive-summary)
- [PROJECT OVERVIEW](#project-overview)
- [BUSINESS PROBLEM](#business-problem)
- [DATA SOURCE](#data-source)
- [DATA PREPROCESSING](#data-preprocessing)
- [DATA ANALYSIS](#data-analysis)
- [RECOMMENDATION](#recommendation)

## Executive Summary

This project demonstrates how data can be translated into clear business recommendations to support market entry decisions for a railway travel startup. Using global development and transport indicators, the analysis evaluates rail passenger demand, infrastructure maturity, economic strength, and ease of doing business to identify countries with the strongest commercial potential.

The work prioritises practical business questions over technical complexity, combining multiple indicators into a coherent decision framework. Visual dashboards and comparative charts are used to highlight trade-offs between demand, economic viability, and operational feasibility. The outcome is a structured, evidence-based recommendation that mirrors how business analysts support strategic planning, investment decisions, and executive discussions.

This project showcases core business analyst capabilities: problem framing, metric selection, insight generation, and stakeholder-ready communication.
## PROJECT OVERVIEW 
This is a **data analytics project** that helps determine the best country to launch a new railway travel company based on global economic and rail usage metrics. The analysis combines infrastructure, travel demand, economic performance, and business environment factors to support strategic decision-making.

## BUSINESS PROBLEM 

As a newly hired data analyst for a startup railway travel company, the goal was to identify markets with the **strongest potential for success**. 
The key questions addressed are:

- Which countries have the greatest existing rail usage?
- How does rail usage align with economic strength and ease of doing business?
- Which markets offer a balance of infrastructure, demand, and growth potential?

## DATA SOURCE

The analysis uses the **World Development Indicators dataset**, which contains country-level metrics including:

- Passenger distance travelled by rail
- Total length of rail infrastructure
- GDP and GDP per capita
- Ease of doing business score

Download dataset here [World-Development-Indicators dataset.xlsx](https://github.com/user-attachments/files/17147007/World-Development-Indicators.dataset.xlsx)

## DATA PREPROCESSING

- Renamed and simplified fields for clarity (e.g., country, rail lines).
- Converted data types appropriately for numeric and geographic analysis.
- Applied country filters to focus on the latest year (2019) for consistent comparisons. 

## DATA ANALYSIS

Since the highest priority is to identify countries that have a high passenger usage of existing railways, i created a bar chart to see how the countries compare with one another.

### KEY INSIGHTS
- China has the highest passenger distance travelled with 1,438,606
- United States ranks high in having an extensive railway network (i.e 149,489 railways), but only carried 32,483 passengers when considering the total length of existing railways.
![Bar chart](https://github.com/user-attachments/assets/efa42405-1c52-42a8-8a18-b776c055f2de)

- Ten Countries are responsible for carrying over 91% of the distance traveled by passengers worldwide. These same countries contain over 60.1% of the world's rails. These countries, are referred to as the Top 10. I created a set to visualize this analysis as shown below:

![Top 10](https://github.com/user-attachments/assets/8c13d119-1ac8-4ce9-a067-17efaa076cba)

The next top priorities are focused on business-related fields — specifically, the GDP per capita and the ease of doing business. Ideally, we’ll want to set up the business in a country that has a high GDP per capita AND ease of doing business score. 
i created a scatter plot with the Business Score on the x-axis and GDP Per Capita on the y-axis. (Note: i first had to create a calculated field for the GDP Per Capita, which is the GDP divided by the Population.)

![Top 6](https://github.com/user-attachments/assets/5c76ba20-0b40-4898-86c7-39a3dfada52c)
- Of the ten countries previously selected based on rail travel, the selection is narrowed down to six based on the ease of doing business score and the GDP Per Capita.The six (06) countries are : United States, Germany, France, Japan, United Kingdom and Korea Republic.

It would be nice to think about the possibility of future international expansion, ideally meaning i select a country that has neighboring countries that are also promising.
I built a map with the six countries above to see their geographic relationship with one another and to see if there are any countries to remove from the list. 
- The map shows that France and Germany share a land border.

![Map](https://github.com/user-attachments/assets/61065c20-0878-450b-8d0e-9c44c7e89ced)

- Of the two countries that share a geographic proximity, France has a significantly higher number of incoming tourists (i.e 217,877,000) which is roughly 5.5 times as many incoming tourists as Germany, indicating a substantially larger and more lucrative market for rail travel. This significant difference in tourist numbers suggests greater potential for customer base expansion and revenue generation in the rail market.

## RECOMMENDATION
Based on combined indicators of rail usage, business friendliness, and economic performance, the analysis suggests selecting a **country with both high rail travel demand and a strong business environment** as the launch market for the new railway travel service.

France emerges as the top pick. It stands out in passenger volume and extensive rail lines, striking a perfect balance with its robust economy and business-friendly environment. Its geographic location offers potential for international expansion, notably with promising neighboring countries. Moreover, France's exceptional tourist appeal, leading in visitor inflow, presents a lucrative market for rail travel. These combined factors make France the most promising country for establishing the new rail travel company.



[View Dashboard Here](https://public.tableau.com/app/profile/adebayo.adebanjo/viz/RailwayTravelCoyProject/RailwayTravelCoyProject)

## Tools & Technologies

- Excel (data source)
- Tableau(for visualization)
