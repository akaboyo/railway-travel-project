![Railway logo](https://github.com/user-attachments/assets/4bec1009-7af5-4806-89a8-6f9b5d92cfe6)

# Railway Travel Company: Market Entry Analysis
Where should a new railway travel startup launch first? A data-driven market selection analysis using global rail, economic, and tourism indicators.

## VERDICT
**Recommendation: Launch in France.**

France is the only market in the analysis with high rail passenger demand, a strong business environment, a border with another top-6 market (Germany) for future expansion, and ~5.5x the inbound tourist volume of its nearest comparable neighbor — the single largest addressable customer base in the shortlist.

## Executive Summary
This project simulates a real market-entry decision: **as the analyst for a new railway travel startup, which country should we launch in first?**

Using the World Development Indicators dataset, I built a four-stage filter — rail usage → economic strength → business environment → expansion potential — to narrow 200+ countries down to one recommendation. The goal wasn't just to find interesting patterns in the data, but to answer a decision a real executive team would need to make, and to make the trade-offs visible enough that they could challenge it.

**Summary**
- **10 countries** carry 91%+ of global rail passenger volume
- Filtering those 10 by GDP per capita and ease-of-doing-business narrows the list to **6**
- Mapping those 6 geographically surfaces **France and Germany** as the only bordering pair — relevant for future expansion
- Comparing tourism inflow between the two, **France** wins by ~5.5x
- **France** is the recommended launch market

## Table of Contents
- [Business Problem](#business-problem)
- [Data Source](#data-source)
- [Data Preprocessing](#data-preprocessing)
- [Analysis Walkthrough](#analysis-walkthrough)
- [Why Not Germany?](#why-not-germany?)
- [Recommendation](#recommendation)
- [Skills Demonstrated](#skills-demonstrated)
- [Tools](#tools)

## Business Problem

As the newly hired data analyst for a startup railway travel company, my task was to identify the market with the **strongest potential for success**. Three questions drove the analysis:

1. Which countries have the greatest existing rail usage?
2. How does that usage align with economic strength and ease of doing business?
3. Which markets offer the best balance of infrastructure, demand, and growth potential?

## Data Source

The analysis uses the **World Development Indicators dataset**, which contains country-level metrics including:

- Passenger distance travelled by rail
- Total length of rail infrastructure
- GDP and GDP per capita
- Ease of doing business score

Download dataset here [World-Development-Indicators dataset.xlsx](https://github.com/user-attachments/files/17147007/World-Development-Indicators.dataset.xlsx)

## Data Preprocessing

- Renamed and simplified fields for clarity (e.g., country, rail lines).
- Converted data types appropriately for numeric and geographic analysis.
- Applied country filters to focus on the latest year (2019) for consistent comparisons.
- Built a calculated field for **GDP per capita** (GDP ÷ Population), since it wasn't in the raw data

## Analysis Walkthrough
### Step 1 — Who actually uses rail the most?

A bar chart of passenger distance traveled by rail across all countries.

![Bar chart](https://github.com/user-attachments/assets/efa42405-1c52-42a8-8a18-b776c055f2de)

<img width="698" height="440" alt="Image" src="https://github.com/user-attachments/assets/8d3cee89-663a-4f04-ae4d-3dc837939100" />

**Insight:** 
- China has the highest passenger distance travelled with 1,438,606
- The U.S., despite having one of the largest rail networks by length (149,489 km), carries a surprisingly small share of passengers relative to that infrastructure — a network-size-to-usage mismatch worth flagging for anyone assuming "more track = more passengers."

### Step 2 — Who dominates global rail usage?

Ten countries carry **91%+** of all rail passenger distance worldwide and hold **60.1%** of the world's total rail infrastructure.

![Top 10](https://github.com/user-attachments/assets/8c13d119-1ac8-4ce9-a067-17efaa076cba)

**Insight:** 
Rail demand is heavily concentrated — this isn't a fragmented global market, it's a short list of countries worth evaluating further.

### Step 3 — Which of those 10 are actually good places to run a business?

![Top 6](https://github.com/user-attachments/assets/5c76ba20-0b40-4898-86c7-39a3dfada52c)

**Insight:** 
Six countries stand out on both dimensions: **United States, Germany, France, Japan, United Kingdom, South Korea.** High rail demand alone is not enough - a market also has to be economically strong and easy to operate in.

### Step 4 — Which of the 6 sets up best for future expansion?

Mapping the six finalists to check for geographic proximity — a market with a friendly, promising neighbor is more attractive for a multi-country expansion roadmap.

![Map](https://github.com/user-attachments/assets/61065c20-0878-450b-8d0e-9c44c7e89ced)

**Insight:** 
Only **France and Germany** share a land border. That single fact reshapes the decision — everything from here is a head-to-head between those two.

### Step 5 — France vs. Germany: the tiebreaker

<img width="983" height="489" alt="Image" src="https://github.com/user-attachments/assets/8304b951-e7cb-463a-9e2a-bed08af16282" />

**Insight:** 
France draws **217.9M inbound tourists** — roughly **5.5x** Germany's volume. That's a materially larger pool of potential rail customers on day one, not just a marginally better score.

## Why Not Germany?

Germany passed every earlier filter — strong economy, easy to do business, borders France for expansion — so it's the natural pushback question. It loses on the metric that matters most for a *travel* company: addressable customer volume. France's tourist inflow is large enough that it isn't a close call, and the shared border means Germany isn't off the table — it's a logical **Phase 2** market once France is established.

## Recommendation

Based on combined rail demand, business environment, and tourism potential, **France** is the strongest launch market:

- **Demand:** Top-10 in rail passenger volume with strong existing rail infrastructure
- **Business environment:** High GDP per capita, high ease-of-doing-business score
- **Expansion runway:** Land border with Germany, the next-best market in the shortlist
- **Market size:** Largest inbound tourism base among the finalists (~5.5x Germany's)

[Explore the full Interactive Dashboard on Tableau](https://public.tableau.com/app/profile/adebayo.adebanjo/viz/RailwayTravelCoyProject/RailwayTravelCoyProject)

## Skills Demonstrated

`Data Cleaning & Preprocessing` • `Calculated Fields` • `Funnel / Elimination Analysis` • `Comparative Analysis` • `Geospatial Analysis` • `Dashboard Design` • `Data Storytelling` • `Stakeholder Communication` • `Business Recommendation Writing`


## Tools
- **Excel** - data source and preprocessing
- **Tableau** - visualization and interactive dashboard

