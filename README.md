# Google Data Analytics Capstone: Rider Behavior Analysis
Author: Madan Timilsina
Date: June 17, 2026
[Click here to view my interactive Tableau Dashboard]([https://public.tableau.com/shared/PZQBR6HJ3?:display_count=n&:origin=viz_share_link](https://public.tableau.com/app/profile/madan.timilsina/viz/Cyclisticdatavisualization/numberofride))

## Background & Business Task
Cyclistic is a premier bike-share program in Chicago featuring over 5,800 bicycles across more than 600 docking stations. The company offers two main pricing plans: single-ride or full-day passes for Casual Riders, and long-term subscriptions for Annual Members. Because annual memberships are more profitable, the primary goal of this analysis is to provide actionable insights to support a marketing strategy that converts casual riders into annual members. This is achieved by analyzing customer interaction history and purchase behavior data.

## Data Source & Methodology
* Data Provenance: The data was sourced from Motivate International Inc. via the divvy-tripdata public bucket.
* Timeframe: The dataset covers a 13-month period from May 2025 to May 2026, consisting of 13 CSV files with 6,351,159 total rows.
* Limitations: For privacy reasons, the data contains no personal identifiable information, meaning rides cannot be linked to individual users.
* Tools Used: Python (Pandas) was utilized for efficient data cleaning and manipulation, while Tableau Public was used for high-impact visualization.

## Data Cleaning Summary
* Removed 6,447 rides missing end latitude and end longitude coordinates.
* Engineered new columns including ride_length, hours, day_of_week, and months
* Created a station_name_status column to track missing station entries.
* Removed 29 rides with duplicate ride_id values.
* Removed 124,904 rides with invalid ride lengths (negative, zero, under 1 minute, or over 48 hours)
* Final Dataset: 6,219,779 valid rides.

## Key Insights
* Usage Intent: Members take almost double the total number of rides than casual riders, indicating they use the service for regular commuting or point-to-point utility. Conversely, casual riders ride nearly twice as long per trip, pointing toward leisure, recreation, or weekend tourism
* Weekly Trends: Casual rider usage concentrates heavily on the weekends, whereas member usage is spread evenly across the weekdays.
* Seasonality: Both rider demographics show peak usage in May, with the most popular time of day being around 5:00 PM.
* Equipment Preferences & Behavior: Electric bikes are the most preferred choice for both groups. Interestingly, classic bikes have almost no missing station names, while electric bikes have a nearly 50/50 split between complete and missing station data. This indicates that the built-in locking mechanism of electric bikes allows users to park them anywhere, which likely drives their higher popularity.

## Strategic Recommendations
* Introduce a Weekend Pass Membership: Create a specialized membership tier targeting casual riders whose usage peaks massively on Saturdays and Sundays.
* Launch an Electric Bike Summer Promotion: Deploy a marketing campaign during peak months (like May) that heavily features electric bikes, capitalizing on the casual riders' strong preference for this rideable type.
* Implement a "Ride to Own" Credit System: Allow casual riders to apply their accumulated single-ride or daily-pass fees toward the cost of an annual membership, visually demonstrating their yearly savings to encourage upgrades.
