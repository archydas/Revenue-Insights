# Revenue-Insights
Power BI Dashboard: Revenue Insights for Hospitality Industry
This Power BI dashboard provides a comprehensive analysis of revenue performance in the hospitality industry. It is designed to offer key insights into room occupancy, revenue trends, seasonal performance, and customer segmentation.
## Objective:
The dashboard aims to provide clear and actionable insights into revenue performance, room bookings, occupancy rates, and seasonal trends within the hospitality sector.
## Data Source: 
The dataset consists of historical booking data from a hotel chain, including information about room types, booking channels, customer demographics, revenue generated per booking, and stay durations.
## Features and Insights:
Revenue: To get the total revenue_realized
Occupancy %: Occupancy means total successful bookings happened to the total rooms available(capacity)
ADR : It is the ratio of revenue to the total rooms booked/sold. It is the measure of the average paid for rooms sold in a given time period.(Average Daily Rate)
RevPAR: (Revenue Per Available Room) RevPAR represents the revenue generated per available room, whether or not they are occupied. RevPAR helps hotels measure their revenue generating performance to accurately price rooms. RevPAR can help hotels measure themselves against other properties or brands.
DBRN:(Daily Booked Room Nights) This metrics tells on average how many rooms are booked for a day comsidering a time period.
DSRN: (Daily Sellable Room Nights)  This metrics tells on average how many rooms are ready to sell for a day considering a time period.
DURN:(Daily Utilized Room Nights) This metrics tells on average how many rooms are successfully utilized by customers for a day considering a time period.
## Methodology
1. Data Cleaning and Preparation:
   a. Cleaned the data by removing irrelevant or incomplete records and handling missing values.
   b. Used Power Query to aggregate revenue data by day, month, and year for time-based analysis.
2. Data Modeling :
   a. Created relationships between different tables (e.g., bookings, rooms, customers) to allow for seamless cross-filtering and exploration.
   b. Calculated fields for KPIs like RevPAR, ADR, and Occupancy Rate using DAX (Data Analysis Expressions).
3. Performed DAX Calculations:
   a. For example : Revenue = SUM(fact_bookings[revenue_realized])
   b. ADR = DIVIDE( [Revenue], [Total Bookings],0)
   c. RevPAR = DIVIDE([Revenue],[Total Capacity])
4. Visualizations: Created line charts for Revenue trend by metrics, RevPar by week no and day type , DSRN by week no , Occupancy % by week no and day type , ADR by week no. Created bar chart for Realisation% and ADR.
## Key Challenges
Data Volume: Handling large datasets with thousands of records posed a challenge, which was managed by aggregating data at higher levels (e.g., monthly or yearly).
## How to use 
Power BI Report File (.pbix): The Power BI file is available in this repository for download. Open it with Power BI Desktop to explore the insights.
## Future Improvements 
1. Predictive Analytics: Incorporating machine learning models to forecast future revenue based on past trends and external factors (e.g., holidays, events, weather conditions).
2. Real-time Data Integration: Integrating real-time booking and revenue data to provide live insights.
## Conclusion 
This dashboard offers critical revenue insights into the hospitality industry, enabling hotel managers and decision-makers to track performance, optimize pricing, and target specific customer segments. It serves as a powerful tool for driving operational efficiency and increasing profitability.
















