---
layout: default
title: Assignment 2 (02806) - Investigation of Correlation Between Narcotic and Assault Incidents in San Francisco
---


# Introduction

Due to the recent opioid crisis, we decided to analyze the historical data for drug usage and assaults in San Francisco. We use the SFPD dataset as well as outside information about San Francisco and try to understand the phenomenon as well as the causes of the issue. First, we compare the instances of drug occurrences and assaults over time and across districts and then try to forecast the trend of future patterns using linear regression. In addition, look for answers outside the dataset into external elements that could explain our findings.


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

To understand the problem thoroughly, the spatial element
is very important. Our analysis shows that there is no clear correlation between drug crimes and assaults, and assaults are relatively equally
spread across the city hence our focus on drug arrests. After data normalization, we color the districts with the
highest degree of drug-related arrests in a strong red color,
and the ones with lower amounts in white with the data
spreading from 2003 to 2017. \\


<iframe src="choropleth_mapbox.html" style="width:100%;height:600px;border:none;"></iframe>

\\
In general, there is a clear trend of reduction of drug-related
crimes in the city except for the period during the financial
crisis of 2008. Norther-eastern districts of the city have larger rates and
these are Tenderloin, Northen, and Mission. The main reason
behind this is that this area is the city center and thus has a
larger population proportion and flow. When dwelling into the
history of Tenderling, the district with the highest proportion of
drug-related crimes, we find clear social and economic factors:
many entertainment venues, high prostitution levels, and a big
concentration of services for the homeless and people with
substance abuse problems. However, when exploring additional factors such as social policies, urban development, and community data, we find
that our conclusion lacks the bigger picture. Hence, we
recommend using a wider approach in analyzing the
phenomena especially due to the current opioid crisis.  

# Prediction of Future Crime Occurences

We did a linear regression analysis to really dig into the trends of two different kinds of crimes: 
drug/narcotic incidents and assaults, looking at the years from 2004 to 2016. We made a graph that 
shows how many times these crimes happened each year. For drug/narcotic incidents, we used blue 
dots on the graph, and it showed that these crimes went down from about 12,000 times in 2004 to 
just over 6,000 times by 2016, so the line on the graph is going down. On the other hand, the red 
dots for assaults went up from around 6,000 to 10,000 times in the same period, so their line on 
the graph goes up.

<iframe src="crime_regression_plots2.html" style="width:100%;height:600px;border:none;"></iframe>

When we drew lines through these dots to summarize the trends (those are the regression lines), 
it looked like these two types of crimes weren’t really related to each other. Instead, they seemed 
to be going in their own directions. On average, drug-related crimes were decreasing by about 500 
incidents every year, while assault cases were going up by about 333 incidents each year. This 
shows how complicated these crime trends can be, and that there might be different reasons that impact
each type of crime.

# Conclusion



