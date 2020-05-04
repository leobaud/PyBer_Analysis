# PyBer Analysis Report

## Background and Results

V. Isualize has requested a new assignment, one that will require the use of everything learned to solve a new challenge: creating a summary DataFrame of the key metrics for the ride-sharing data by city type; creating a multiple-line graph that shows the total fares for each week by each city type; and submitting a written report on the results of the new analysis, challenges encountered and overcame, and any future recommendations for analysis.

### Purpose

The purpose of this analysis, is to get a better picture of the total amount of fares, rides and drivers per city type by using the provided city data and ride data.

### Technical Analysis

By combining both data sets we are able to create a single DataFrame containing each specific ride ID with its city, fare amount, driver count and type of city. With dataframe it makes we can get the total amounts of fares, rides and drivers. Having the totals for each item, we can then get the average fares per single ride and single driver. Once we have each of the data sets we need, we can create a new dataframe that shows the total amounts we calculated by city type. In the first deliverable you can see for each city type, the total of rides,  total of drivers, total fares, average fare per ride and average fare per driver, during the analyzed period of time (January 2019 to May 2019).

### Results

As it can be observed in the dataframe created the difference of total rides for the Rural city type varies between 5 and 13 times the Suburban and Urban city types. Because of this difference, the average fare amount per ride in a rural city is $10 more expensive than the average fare amount in the urban area. 

## Challenges Encountered and Overcome

On analyzing the data, there where some challenges that we were able to overcome. 

1) The Date column from the database provided in the csv file had to be formatted from the Jupyter Notebook, so that it could contain the data type we needed for the analysis. The column was originally recognized as an object, hence the pandas date functions werent recognizing the data. 

2) Another challenge we overcame was when trying to count the total amount of drivers. Pandas wasn't recognizing the drivers count in the merged dataframe as a sum. . 

3) Finally when creating the linear plot, we resampled the data to have the sum of fares per week, per city type and created a new dataframe. There was a bit of a stragle to show each week per month in the x-axis. 

### Technical Analyses Used

1) We were able to solve this issue by changing the data type to DateTime. The column was originally recognized as an object, hence the pandas date functions werent recognizing the data.

2) we used the original city data to workaround this issue.

3) Thankfully we were able to solve it as well by specifying the x-axis information using the new dataframe created.

## Recommendations and Next Steps

Because of the low demand of rides in the rural cities, the fare amounts are higher. If rural cities had more rides and drivers, the fare amounts would decrease. People in the urban areas need much more transportation services so PyBer is doing really good in this niche. Suburban rides can be increased by trying to lower fares or making ride promotions for more clients to use the service. On the rural side, we could implement a partnership with businesses in the rural areas to offer ride from home to business for more people to use the service and not there own tranportation modes.

### Recommendations for Future Analysis

Information about ride times, ride routes and frequency of same users can help implement an startegy to help the business grow in this areas. By analysis routes we can try to increase the number of drivers near the route area. Also knowing the frequency of service by users we can develop promotional fares for customers. 
