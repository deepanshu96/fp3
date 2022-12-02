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

While we visualized the hate crime trend at a country level, lets now have a look at how the city of Chicago fares in hate crimes across few of the most frequent bias motivators such as race/ethnicity, gender identity, sexual orientation, and religion. Just like the rest of the country and the world, the total number of crimes have only increased with time but there has been an almost 200% increase in crimes related to race/ethnicity and gender identity related cases have been newly reported in the past 5 years. This trend is corroborated by our first visualization above where we saw that the total number of hate crimes have approximately increased by 25% in 2020 in comparison to 2019.

<img src="{{ site.baseurl }}/assets/json/v33.png" alt="drawing" width="80%"/>

# Visualization 3

We attempted to have a look on the hate crime data of another country to create comparison and extract inferences. Here, we have focused on England and Wales as these are the two countries with maximum number of hate crimes reported within United Kingdom. In the visualization we can see total number of hate crimes in past eleven years across different categories. Hate crimes committed against a person due to their race and sexual orientation are two topmost reported category of hate crime. In 2021, the total of 67% and 16% hate crimes were reported against race and sexual orientation respectively.

<img src="{{ site.baseurl }}/assets/json/v22.png" alt="drawing" width="80%"/>

# Conclusion

As we have seen above, irrespective of the hate crime data at a city, country or global level, it has been on a constant rise across and the onus is on us as citizens to be more aware of our surroundings and be responsible. We have to be more conscious about our own biases instilled within us by the society at large.

### References
 [[1] https://www.statista.com/statistics/284160/hate-crimes-in-england-and-wales-by-motivating-factor/](https://www.statista.com/statistics/284160/hate-crimes-in-england-and-wales-by-motivating-factor/)<br> 
[[2] https://home.chicagopolice.org/statistics-data/data-dashboards/hate-crime-dashboard/](https://home.chicagopolice.org/statistics-data/data-dashboards/hate-crime-dashboard/) <br>
## Search The Data & Methods


<!-- these are written in a combo of html and liquid --> 
 
<div class="left">
{% include elements/button.html link="https://crime-data-explorer.fr.cloud.gov/pages/downloads" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/deepanshu96/fp3/blob/main/group_24_final_project_part_3.ipynb" text="The Analysis" %}
</div>

