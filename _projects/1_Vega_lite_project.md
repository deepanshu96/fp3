---
name: Final Project Group No. 24
tools: [Python, HTML, vega-lite]
image: assets/json/aa.png
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


<h1 align="center">
 Hate Crime on the rise
</h1>
##### Group 24: Team Members
##### Akshya Yadav
##### Deepanshu Malhotra
##### Harsh Baberwal
##### Shruti Jain
<br> 

A hate crime can be defined as an offense committed against a person based on pre-conceived biases about their identity such as race, gender, sexual orientation, ethnicity, etc. These perpetual crimes have lately been on the rise after certain global incidents. These recent incidents of hate crimes motivated us to find the underlying trends of such crimes (if any) in the United States of America. 
All sources have been linked at the bottom of the article.


# Visualization 1
We have used the crime data available with the Federal Bureau of Investigation (FBI) as it is a reliable source of information.
In the dashboard below, you would see that the first visualization is a geographical map of the United States of America in which we have plotted the total no. of hate crimes reported in the dataset between the years 1991 and 2020 whereas the corresponding line chart is a time series plot for the same data. 
* You have the ability to select one or more states from the map to see the hate crime trend across the years for those states(use shift + click)
* The color scale for the map depicts the total no. of cases, the darker a state is marked, the more no. of hate crimes have been reported there
* The user has the ability to select a specific state or multiple(use shift + click) and see the hate crime trend in those states for the years 1991-2020

<vegachart schema-url="{{ site.baseurl }}/assets/json/Viz1.json" style="width: 100%"></vegachart>



# Visualization 2

We have used ordinal encoding type for the X axis because that has the building status mapped. As for the Y axis, we have calculated the sum of the square footage field from the dataframe for the city selected by the user.
We came across another way of plotting using Altair using the chart function and used that as we were enable to activate interactivity using the ".from_dict" trait (citation has been added above)
One thing we were not able to achieve was for cities which have only 1 type of building status related data, we were unable to display the other empty building status on the X axis.
Moreover, altair did not let us enable interactivity for more than 5000 rows, so we had to create a subset of the original dataframe to include only <5000 rows
Additionally, we tried but could not sort the list of cities in the dropdown
We also tried to validate the interactivity by using pandas to create a pivot table for the cities to verify the total sum of square footage values for each city for each building status type
This visualization can provide assistance to the Real Estate Sector in generating the blue-print of the city.

<img src="{{ site.baseurl }}/assets/json/v22.png" alt="drawing" width="80%"/>

# Visualization 3

We have used ordinal encoding type for the X axis because that has the building status mapped. As for the Y axis, we have calculated the sum of the square footage field from the dataframe for the city selected by the user.
We came across another way of plotting using Altair using the chart function and used that as we were enable to activate interactivity using the ".from_dict" trait (citation has been added above)
One thing we were not able to achieve was for cities which have only 1 type of building status related data, we were unable to display the other empty building status on the X axis.
Moreover, altair did not let us enable interactivity for more than 5000 rows, so we had to create a subset of the original dataframe to include only <5000 rows
Additionally, we tried but could not sort the list of cities in the dropdown
We also tried to validate the interactivity by using pandas to create a pivot table for the cities to verify the total sum of square footage values for each city for each building status type
This visualization can provide assistance to the Real Estate Sector in generating the blue-print of the city.

<img src="{{ site.baseurl }}/assets/json/v33.png" alt="drawing" width="80%"/>

### References
 [[1] https://www.statista.com/statistics/284160/hate-crimes-in-england-and-wales-by-motivating-factor/](https://www.statista.com/statistics/284160/hate-crimes-in-england-and-wales-by-motivating-factor/)<br> 
[[2]https://home.chicagopolice.org/statistics-data/data-dashboards/hate-crime-dashboard/](https://home.chicagopolice.org/statistics-data/data-dashboards/hate-crime-dashboard/) <br>
## Search The Data & Methods


<!-- these are written in a combo of html and liquid --> 
 
<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/akshyay2/HW-10/blob/main/Group11_Homework_10_Final%20(1).ipynb" text="The Analysis" %}
</div>

