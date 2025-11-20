---
name: Plot 2
tools: [Python, HTML, vega-lite]
image: assets/pngs/chart2.png
description: This is the second plot that is interactive!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Square Footage for each Agency over the years



<vegachart schema-url="{{ site.baseurl }}/assets/json/chart2.json" style="width: 100%"></vegachart>

This visualization is focusing on the total square footage each agency has taken over a certain amount of years. For this plot, I also chose respective encoding types like Nominal for Agency Names and Quantitative for Square Footage and Years. I did add color this time to the Agency Names category because with the amount of agencies changing over the years, it helps to see the difference among agencies when selecting different time periods. Also, I had scaled the years to not include the default 0 so as to not confuse the plot and data. Thus, I also only included the data points that had more than the 0 value.

For the interactivity, I had it so that the user can select the data of a certain period of years to look at in the bottom plot and have the respective agencies that acquired buildings during those years show up on the top plot. It allows the user to be able to see what agencies were acquiring buildings over certain years, as well as, which ones acquired more square footage compared to others in certain timespans.


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="Python Notebook" %}
</div>

