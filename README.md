# W5-Matplotlib-PyBer_Analysis

## Overview of the Analysis
This goal of this project was to analyze PyBer's (a ridesharing company) rideshare data from January to early May of 2019 and create a compelling visualization to understand revenue generation from different city types. For this analysis we split cities into three categories, Urban, Suburban and Rural. We combined data from two CSV files into a single dataframe and utilized Pandas and Matplotlib to parse through the data. 

## Resources
Python 3.7
Jupyter Notebook
Pandas
Matplotlib.pyplot

## Results:
In the first part of our analysis, we utilized a merged dataframe and the groupby method to create an overvie of the number of rides, the average fare and the average fare per driver for each city type. As shown in the figure below, there were considerably more rides and more revenue generated for the urban cities. However, the average fare prices and fare per driver is lowest for the urban rides. This suggests riders in suburban and rural settings are making longer but fewer trips. 

![fig1](https://user-images.githubusercontent.com/81983110/119283573-7ba4eb80-bc0b-11eb-82e8-4661671ae8f0.png)

In the second part of our analysis we restructured our data using the groupby method again to create a new dataframe by type and then by date. We created a pivot table with data as the index and used the resampling method to sample the sum of fares within a week for each city type. Using Matplotlib.pyplot, we graphed the results into the figure shown below. 

![Pyber_Challenge_Figure](https://user-images.githubusercontent.com/81983110/119284035-b8bdad80-bc0c-11eb-92ed-d5b559f4c428.png)

As shown in the figure below, the weekly revenue from January through April for each city type remains relatively stable. We observe a small spike across all city types in late February but the majority of fluctuation is within $300-500 week over week. This suggests that within the timeframe sampled, there is no major 'peak ridership week' to consider. We also observed that revenue is lowest for Urban and Suburban cities right at the beginning of the year.

## Summary:
Based on the results above, we can begin to draw some conclusions about PyBer's profitability and potential next steps as a business. There are a few potential options to drive increased usage of PyBer based the analysis above. 
#### Method 1: Dropping Prices in the First Half of January 
We observed that revenue for Urban and Suburban cities is lowest right at the beginning of the year. Given that this is the holiday season, this suggests that riders are potentially using other methods of transportation or generally breaking from routine. Offering discounted prices during this time might encourage riders to use the service more frequently, even for smaller trips. We could verify this drop in ridership using similar methods to those outlined above, but focusing on number of rides when resampling by week. 
### Method 2: Increasing Incentives for Suburban and Urban Drivers
We observed that while the average fare per ride increases between Urban to Suburban to Rural, the average fare per driver increases much faster. For example, the fare difference for Urban and Suburban trips is about $6.50, whereas the fare per driver difference is about $23. By increasing the number of drivers in Suburban cities, PyBer can increase it's service levels in those areas and maximize potential demand.
### Method 3: Increase Prices for Urban Rides
Of the total number of trips sampled, Urban rides made up nearly 70% of all trips. The most impactful changes to PyBer's bottomline will come from increased profitability from these rides, however the fare per ride is the lowest in this group. This is likely because urban riders are traveling less distance so the pricing could be adjusted to account for this difference. PyBer could also rollout new services to these group first when hoping to maximize exposure to a large group of customers.
