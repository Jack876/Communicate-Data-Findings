# Communicate-Data-Findings

# Ford GoBike System Dateset Exploration
## by YIJJIE ZHANG

# (Dataset Exploration Title)
## by (your name here)



## Dataset
Ford GoBike System Dataset is a dataset that contains trip data from Lyft's bike service for public use. This dataset includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. Variables including, trip duration, start time and end time with date, start station and end station names, start and end coordinates, customer type, etc.

Firstly, I use Python visualization libraries to systematically explore this dataset, starting from plots of single variables and building up to plots of multiple variables. Then I produce a short presentation that illustrates interesting properties, trends, and relationships that I discovered in the dataset. 

## Summary of Findings

Yearly Change: The riding count increased dramatically from year 2017 to 2018, then gain moderately in 2019. This is a good sign for the company.    
Monthly Change: From the month perspective, September and October are the two busiest month of the years. Then comes July and August. Obviously, summer and autumn are the best seasons to enjoy outdoor riding.
Daily change: The riding happened evenly during every month if I dropped out the outlier of the 31rd. In other words, during the 30 days of every month, the riding frequency did not change much. Furthermore, I think this is not the real life difference. The outlier happened just because only about 6 months has the 31rd day, other months has not the 31rd day. The calendar reason causes the strange value of 31rd day , which does not necessarily mean the riding count is low on this day.
Hourly Change: There are two peaks in everyday operation. One is 8-9am and the other is 17-18pm. This is in line with the common working hours. It is natural to have the lowest count from 0 to 5 in late night.

Riding Distance. When considering bike riding distance, we can see there is a maximum value of 12,803,570. While most values are under 4000. By zoom in the graph, I find 75% values are 2167. Interestingly, the minimum value is 0, which means some users rent bikes but did not used them at all.
Riding Time. When considering duration minutes, we can see there is a maximum value (1520 minutes =25.33 hours). While most values are under 2000 minutes. By zoom in the graph, I find 75% values are under 14.76 minutes. Specifically, most riding time is 5-10 minutes. I also notice there are some strange outliers, like the max value is 1520 minutes (25.33 hours). This is a very interesting number since nobody would rent a bike and keep on riding for more than 24 hours. I guess a possible reason is some customers did not remember to return their bikes until the next day.

User type and riding distance. There are not much difference between customer group and subscriber group when considering their riding distance. They have similar means and percentiles. The only difference is customer group has a few bigger outliers than the subscriber group has. This might indicate whether subscribing or not does not impact peoples' riding behavior. The possible reason is renting cost is not a big deal for most customers.

User type and riding time. The median riding time of customer group is slightly higher than that of the subscriber group, which is a bit contradict to our institution. The maximum values for both groups are almost the same. This might indicate subscribing service does not necessarily increase the riding time. The possible reason is people use the service just for actual needs. Subscribers would not ride more frequently than other customers.
Further investigation of the two by multivariate exploration shows customer group has much higher average riding time comparing to subscriber group. Another point is customer group also has much higher variation from month to month, while the subscriber group line tend to be quite flat. It may suggest that the company should pay more, at least equal, attention and resource to the consumer service of non-subscribers.

Riding time and distance. When riding time (duration_min) increases, most of distance values would not have linear increase, but keep on the same level except for some outliers. Most riding distance happen under 15000. This is interesting because I assumed the two factors may had positively linear relationship. It may show during the time from begin to bike sharing end the bikes are not always in motion status. 

Distance vs Month. From January to April, the riding distance increases steadily. After April, it dropped temporarily for only one month then moved up gradually to the peak on November. Then it decreased in the last month during the period of three years. 

Yes, I plan on bringing them into my explanatory presentation.


## Key Insights for Presentation

1.	When is the important time for the bike-sharing company?
Yearly Change: The riding count increased dramatically from year 2017 to 2018, then gain moderately in 2019. This is a good sign of development for the company.    
Monthly Change: From the month perspective, September and October are the two busiest month of the years. Then comes July and August. Obviously, summer and autumn are the best seasons to enjoy outdoor riding.
Daily change: The riding happened evenly during every month if I dropped out the outlier of the 31rd. In other words, during the 30 days of every month, the riding frequency did not change much. Furthermore, I think this is not the real life difference. The outlier happened just because only about 6 months has the 31rd day, other months has not the 31rd day. The calendar reason causes the strange value of 31rd day , which does not necessarily mean the riding count is low on this day.
Hourly Change: There are two peaks in everyday operation. One is 8-9am and the other is 17-18pm. This is in line with the common working hours. It is natural to have the lowest count from 0 to 5 in late night.

2.	Does user type impact riding time?
User type and riding time. The median riding time of customer group is slightly higher than that of the subscriber group, which is a bit contradict to our institution. The maximum values for both groups are almost the same. This might indicate subscribing service does not necessarily increase the riding time. The possible reason is people use the service just for actual needs. Subscribers would not ride more frequently than other customers.
Further investigation of the two by multivariate exploration shows customer group has much higher average riding time comparing to subscriber group. Another point is customer group also has much higher variation from month to month, while the subscriber group line tend to be quite flat. It may suggest that the company should pay more, at least equal, attention and resource to the consumer service of non-subscribers.

## Feedback from others

I showed the dataset analyses to one of my friend who is an accountant. At the beginning, he is surprised that I could got so much interesting information from the original bike sharing data. I explained that this is the power and attraction of data analysis, as well as how the data analysis help modern business develop. Then he is confused by some statistical detail I used in the graph. For example, he already mixed the percentiles meaning of box plots which he studied in the college many years ago. Besides this, he might need introduction of violin graph. A good suggestion from him is I should keep good balance between meaningful explaining words and advanced statistical tools.
