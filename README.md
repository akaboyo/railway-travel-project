# Railway Travel Company 

## Project Overview: 
I have just been hired as a data analyst to help start a company that will focus on booking railway travel.

I have access to a dataset that contains valuable country information, including gross domestic product (GDP), the extent of railway infrastructure, ease of doing business score, and more.

I have been asked to use this data to make a data-driven recommendation as to which country the business should select to launch its startup.

## PROBLEM STATEMENT

To succeed in this endeavor, i considered various factors that can influence the business's success such as:

- Should Railway Travel Coy prioritize a country with a high GDP or one with a favorable ease of doing business score?

- How might the presence of railways and the number of passengers affect the business?

- How important is the number of incoming international visitors?

The team has shared the following factors with me, in order of importance:

- Current usage of the existing railways.

- Total length of existing railways.

- GDP per capita.

- Ease of conducting business.

## DATA SOURCE

The dataset used for this analysis is World Development Indicators which contains 1,521 rows and 8 fields, and this is attached below:

[World-Development-Indicators dataset.xlsx](https://github.com/user-attachments/files/17147007/World-Development-Indicators.dataset.xlsx)

A closer look at the dataset shows that each country appears multiple times and there are multiple years of data. To get the most up-to-date information, i filtered on 2019. Since this filter is to be applied throughout the entire workbook and not just a single visualization, i had to set this up as a data source filter. This left me 217 rows of 2019 data to analyse.

## DATA PREPROCESSING/TRANSFORMATION

Some fields of the dataset were renamed and transformed so as to be suitable for analysis:

### Renaming Fields
- Country Name → Country: Simplified for clarity.
- Time → Year: Standardizing the term to represent the specific year for analysis.
- Ease of Doing Business Score → Business Score: The name has been shortened to keep the focus on the business metric.
- Railways, Passengers Carried → Passenger Distance Traveled: Renamed to better reflect the type of data.
- ternational Tourism, Number of Arrivals → Incoming Tourists: Simplified for ease of interpretation.

### Assigning Data Types
- Country: Identified as a Geographic field, indicating that this column contains location-related data.
- Year: Set as a Date type, suggesting this field is used for time-based analysis.
- GDP: Assigned as a Number (whole), indicating GDP values are non-decimal whole numbers.
- Business Score: Defined as a Number (decimal), indicating the data has precision and requires decimal values.
- Rail Lines: Marked as a Number (decimal), also requiring decimal precision.
- Passenger Distance Traveled: Number (decimal) type, where distance data likely includes decimals.
- Incoming Tourists: Categorized as Number (whole), implying the tourist count is an integer.

### Organizing the Fields
I placed a few related fields together and organized them into the following folders:

- Business

     - Business Score

     - GDP

- Country

     - Country

     - Population

- Travel

     - ncoming Tourists

     - Passenger Distance Traveled

     - Rail Lines

## DATA ANALYSIS/VISUALIZATION

Since the highest priority is to identify countries that have a high passenger usage of existing railways, i created a bar chart to see how the countries compare with one another.

### KEY INSIGHTS
- China has the highest passenger distance travelled with 1,438,606
- United States ranks high in having an extensive railway network (i.e 149,489 railways), but only carried 32,483 passengers when considering the total length of existing railways.
![Bar chart](https://github.com/user-attachments/assets/efa42405-1c52-42a8-8a18-b776c055f2de)

- Ten Countries are responsible for carrying over 91% of the distance traveled by passengers worldwide. These same countries contain over 60.1% of the world's rails. These countries, are referred to as the Top 10. I created a set to visualize this analysis as shown below:

![Top 10](https://github.com/user-attachments/assets/8c13d119-1ac8-4ce9-a067-17efaa076cba)

The next top priorities are focused on business-related fields — specifically, the GDP per capita and the ease of doing business. Ideally, we’ll want to set up the business in a country that has a high GDP per capita AND ease of doing business score. 
i created a scatter plot with the Business Score on the x-axis and GDP Per Capita on the y-axis. (Note: i first had to create a calculated field for the GDP Per Capita, which is the GDP divided by the Population.)

