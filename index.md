---
layout: default
title: Assignment 2 (02806) - Investigation of Correlation Between Narcotic and Assault Incidents in San Francisco
---


# Introduction

This is a normal paragraph following a header. 


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

Ovdje text o lokacijama plus slika plus ovo je test

<iframe src="choropleth_mapbox.html" style="width:100%;height:600px;border:none;"></iframe>


# Prediction of Future Crime Occurences

<iframe src="crime_regression_plots.html" style="width:100%;height:600px;border:none;"></iframe>

We present a detailed linear regression analysis that quantitatively dissects the trends of two 
distinct crime categories: _Drug/Narcotic_ and _Assault_ incidents from 2004 to 2016. The graph plots 
yearly incident counts, with _Drug/Narcotic_ incidents depicted by blue dots, showing a decrease 
from around 12,000 occurrences in 2004 to just over 6,000 by 2016, resulting in a negative slope. In 
stark numerical contrast, the red dots representing _Assault_ ascend from approximately 6,000 
to 10,000 incidents in the same timeframe, resulting in a positive slope. The regression lines, 
serving as a statistical summarization of the data, suggest no evident cross-correlation in the 
quantitative analysis. Instead, they delineate a decoupling of trajectories with an average annual 
decrease of about 500 drug-related incidents versus an average annual increase of roughly 333 
_Assault_ cases, underscoring the complexities and potentially independent drivers behind these criminal 
behaviors.

# Conclusion



