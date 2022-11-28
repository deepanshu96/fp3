---
name: IS 445 DATA VIZUALIZATION
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Homework - 10, Group - 11
## Team Members: 
#### Akshya Yadav
#### Deepanshu Malhotra
#### Shruti Jain

#### We have used the starboard code from Akshya's Homework 9 assignment and built on it as per the homework 10 requirements. In this assignment, we have taken the visualization 1 from the homework 9 and plotted it using the altair library in python. For visualization 2, we have added a dropdown as an interactivity so that the user can change the city according to their preference. This explains our overlap with assignment 9. 

# Visualization 1 
### The aim for this visualization is to understand how the average size of the buildings constructed over the years and how has it evolved over the years because with time, open spaces have reduced and that has resulted in smaller buildings. 
We have used temporal encoding type for the X axis because that has the year value mapped. As for the Y axis, we have calculated the average value of the squar footage field from the dataframe
We first removed the rows which had empty value in the 2 fields-year constructed and square footage. We then filtered only the data for buildings constructed between the years 1800 and 2022
We used the same plot from homework 9 but the width and height encoding in javascript was not working the same way in altair and so we had to use ".properties" trait. We got the solution to this issue from https://coderzcolumn.com/tutorials/data-science/altair-basic-interactive-plotting-in-python
In this line chart, the original color of the plot is green but when we choose the interval, the color of the the graph changes to blue. We were able to make this happen by using colormap. Our aim was to change the color of the selected interval in the plot but we were unable to achieve this is in altair library.
We did not make this interactive. 

<vegachart schema-url="{{ site.baseurl }}/assets/json/Viz1.json" style="width: 100%"></vegachart>



# Visualization 2
### The aim for this visualization is to understand how much space in terms of square footage of buildings is actually in use or not across the various cities of Illinois
We have used ordinal encoding type for the X axis because that has the building status mapped. As for the Y axis, we have calculated the sum of the square footage field from the dataframe for the city selected by the user.
We came across another way of plotting using Altair using the chart function and used that as we were enable to activate interactivity using the ".from_dict" trait (citation has been added above)
One thing we were not able to achieve was for cities which have only 1 type of building status related data, we were unable to display the other empty building status on the X axis.
Moreover, altair did not let us enable interactivity for more than 5000 rows, so we had to create a subset of the original dataframe to include only <5000 rows
Additionally, we tried but could not sort the list of cities in the dropdown
We also tried to validate the interactivity by using pandas to create a pivot table for the cities to verify the total sum of square footage values for each city for each building status type
This visualization can provide assistance to the Real Estate Sector in generating the blue-print of the city.

<vegachart schema-url="{{ site.baseurl }}/assets/json/Viz2.json" style="width: 100%"></vegachart>


## Search The Data & Methods


<!-- these are written in a combo of html and liquid --> 
 
<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/akshyay2/HW-10/blob/main/Group11_Homework_10_Final%20(1).ipynb" text="The Analysis" %}
</div>

