---
layout: default
title: Final Project - lInvestigation of Correlation Between Narcotic and Assault Incidents in San Francisco
---


# Introduction

Due to the recent **opioid crisis**, we decided to analyze the historical data for drug usage and assaults in San Francisco. We use the **SFPD dataset** as well as outside information about San Francisco and try to understand the phenomenon as well as the causes of the issue. First, we compare the instances of **drug arrests** and **assaults** over time and across districts and then try to forecast the trend of future patterns using **linear regression**. In addition, look for answers outside the dataset into external elements that could explain our findings as we found dataset doesn't present the full picture.



# Evolution of Crime Incidence Over Time

The time series of _Drug/Narcotic_ and _Assault_ crimes was analyzed for the following three time intervals/categories: 

* Crime rate per **year**
* Crime rate per **day of week**
* Crime rate per **hour**  

The interactive plot allows the user to observe the barchart for all three time intervals, and to select which crime type will be observed in the barchart. Additionally, the crime count values have been normalised, for easier comparison of the two crime types.

<iframe src="crimes_plot1.html" style="width:100%;height:600px;border:none;"></iframe>

## Crime rate per year

From the yearly plot, it can be observed that the _Drug/Narcotic_ crime is growing each year until 2009, followed by a significant decrease. _Assault_ crime has become more constant over the years. Therefore, from the yearly plot, it can be concluded that there is no correlation between _Drug/Narcotic_ and _Assault_ crimes. 

## Crime rate per day of week

In the weekly plot, it can be observed that the _Drug/Narcotic_ crime has the highest rate on Wednesday, while the crime rate of the _Assault_ is higher on the weekend. Such an outcome is understandable, as the addiction-related crimes will be more evenly spread throughout the week, unlike the assault crimes which occur outside of people's working days. 


## Crime rate per hour

The hourly plot shows a higher similarity in crime rate between the two crime types, mostly due to the natural habits of people. However, in the night hours, there is a higher crime rate of _Assault_, as the attackers are less likely to be spotted while committing the crime.

# Mapping of Crime Occurence

To understand the problem thoroughly, the **spatial element** is very important. Our analysis shows that there is no clear correlation between drug crimes and assaults, and assaults are relatively equally spread across the city hence our **focus on drug arrests**. After data normalization, we color the districts with the highest degree of drug-related arrests in a **strong red color**, and the ones with lower amounts in **white** with the data spreading from **2003 to 2017**.



<iframe src="choropleth_mapbox.html" style="width:100%;height:600px;border:none;"></iframe>

In general, there is a clear trend of **reduction of drug-related crimes** in the city except for the period during the **financial crisis of 2008**. Northern-eastern districts of the city have larger rates, and these are **Tenderloin, Northern, and Mission**. The main reason behind this is that this area is the city center and thus has a larger population proportion and flow. Specifically, **Tenderloin** in the district with the largest amount of Drug/Narcotic related crimes with **4,822 reported related arrests in 2008**.
Interestingly, when comparing SFPD data with personal income data, in assaults there is a similar number increase in all districts, while drug related crimes are moslty in lower-income parts. When dwelling into the history of Tenderloin, the district with the **highest proportion of drug-related crimes**, we find clear social and economic factors: many entertainment venues, high prostitution levels, and a big concentration of services for the homeless and people with substance abuse problems. However, when exploring additional factors such as social policies, urban development, and community data, we find that our conclusion lacks the bigger picture. Hence, we recommend using a wider approach in analyzing the phenomena especially due to the current opioid crisis.


# Prediction of Future Crime Occurences

We used a linear regression to understand into the trends of **drug/narcotic incidents** and **assaults**, looking at the years from **2004 to 2017**. We made a graph that shows how many times these crimes happened each year. For drug/narcotic incidents, we used **blue dots** on the graph, and it showed that these crimes went down from about **12,000 times in 2004** to just over **6,000 times by 2017**, so the line on the graph is going down. On the other hand, the **red dots** for assaults went up from around **6,000 to 10,000 times** in the same period, so their line on the graph goes up.


<iframe src="crime_regression_plots2.html" style="width:100%;height:600px;border:none;"></iframe>

When applying linear regression model, the data clearly shows that two types of crimes aren't related to each other. Instead, they seemed to be going in their own directions. On average, drug-related crimes were decreasing by about **500 incidents every year**, while assault cases were going up by about **333 incidents each year**. This shows how complicated these crime trends can be, and that there might be different reasons that impact each type of crime. 


# Conclusion
In our analysis of correlation between drug and assault related crimes in San Francisco, we discovered patterns and trends across various timeframes and districts showing no clear correlation between the two crime types. Further analysis would be required to understand whether one crime induces another in order to optimize police response and crime prevention. All together, we advocate for a broader analysis of the problem including bigger datasets and other perspectives such as people density in districts at a given time, type of drug, and other information.


 