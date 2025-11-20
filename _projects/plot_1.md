---
name: Plot 1
tools: [Python, HTML, vega-lite]
image: assets/pngs/chart1.png
description: This is the non-interactive first plot!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# County vs Total Square Footage



<vegachart schema-url="{{ site.baseurl }}/assets/json/chart1.json" style="width: 100%"></vegachart>

In this visualization, we are looking at how much total square footage is being covered by buildings in our dataset for each county. I wanted to keep it simple for the first plot and chose to show a normal bar plot with respective encoding types like Quantitative for Square Footage and Nominal for County names. I thought varying in colors would be too much if our main focus is comparing total square footage so I kept the color as default so it's easier to compare and focus on just the total amount of square footage. The only data transformation I had to do for this graph was to allow large datasets to be able to be graphed using vegafusion. Overall, this was the simpler plot to help understand the other plot.



<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/NateLee1494/natelee1494.github.io/blob/master/python_notebooks/HW%205%20Workbook.ipynb" text="Python Notebook" %}
</div>

