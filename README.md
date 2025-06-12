# Hospitality-Doamin
Python Project
Problem Statement:
Atliq has many hotel chains across different cities in india but in the year 2022 they have seen a decrease in their revenue.So they hired a data analyst team to find out the root cause of the issue.

Steps that involved in this project:
1.Exploratory Data Analysis
2.Data Cleaning and Transformation
3.Data Visualization

Exploratory Data Analysis:
During the EDA on the data sets we had few observations:
1.In "no of guest" columns some of the values were in negative.
2.There were null values in 'rating' and 'capacity' columns.
3.There are many outliers in the 'revenue' columns.
4.Dates in 'check_in_date' were not in a consistent format.
5.Highest hotels are in mumbai followed by bangalore

Data Cleaning and Transformation:-
1.Removed the outliers from "revenue" column using 3 standard deviation technique.
2.Replaced the null values from the "capacity" column in fact_aggregated_booking table with mode of the capacity for that particular room category
3.Kept null values of 'ratings' column as it is bcoz rating can be null
4.Added a new column called "occupancy_percentage" in fact_aggeregated_booking table
5.Merged fact_aggregated_table and dim_rooms table(we have merged other tables also based on the analysis)
6.Transformed "check_in_date" into a consistence date format.

Data Visualization:
1.We have used matpotlib,seaborn libraries to visualize the data
2.We have used barcharts,column chart,pie chart,line chart,dougnut chart along with other functions like groupby,agg to get dig deep into the data

Conclusions:
1.Two hotel chan of atliq that is 'Atliq Seasons' and 'Atliq Grands' has the lowest ratings thats why their revenue is also less.In general the average rating of atliq hotels are below 4 which is impacting their buisness.
2.Their 'cancellation_percentage' and 'no show percentage' consists about 30% of their total bookings which means people are booking but due to the reviews they are either cancelling it or not showing at all.
3.Mumbai has the most revenue generating city.
4.The revenue suddenly declined after the month of july but their weekly revenue is not consistent.
5.I can see weekday has more booking_pct than weekends which suggest that donr have any dynamic pricing for weekends.

