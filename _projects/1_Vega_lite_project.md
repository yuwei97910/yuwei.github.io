---
name: Homework10
tools: [Python, HTML, vega-lite]
image: assets/pngs/viz.jpg
description: I know nothing about Jekyll!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# IS445 Assignment 10 - Group 50

- Ching-Yun Huang (ch60@illinois.edu)
- Haocheng Zhong (hzhong11@illinois.edu)
- Thomas Huang (yenshuo2@illinois.edu)
- Yu-Wei Lai (yuwei6@illinois.edu)

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/hw10_1.json" style="width: 100%"></vegachart>
<vegachart schema-url="{{ site.baseurl }}/assets/json/hw10_2.json" style="width: 100%"></vegachart>
```

## Heatmap for the Agency to total floors

<vegachart schema-url="{{ site.baseurl }}/assets/json/hw10_1.json" style="width: 100%"></vegachart>

### Summary
The left plot is the heatmap for the Agency to total floors. Those boxes with deeper colors contain more data. The plot on the right-hand side is the bar chart showing the number of buildings constructed in the years. Both plots are based on HW9, and we connect them together. Users can drag and select data points on the heatmap, and the var chart will show the information about when these buildings were constructed. 

## The distribution of the Square Footage of the records

<vegachart schema-url="{{ site.baseurl }}/assets/json/hw10_2.json" style="width: 100%"></vegachart>

### Summary
For the second visualization, based on the HW9, the histogram summarizes the distribution of the Square Footage of the records. We allow the user to select a range in the top histogram, and the plot below will react to the details based on the range user specified. The default setting of the plot below includes all of the data, which has a huge range to the number over 1,200,000. However, we choose to limit the range to 50,000 for the user selection range because the distribution with a larger number is too sparse. The bin of the top plot is set to 150 with more details, while the bins for the second plot are set to 50.

Below is where we can put some links to both the data and the analysis code as buttons:

```
<div class="left">
{% include elements/button.html link="https://github.com/yuwei97910/yuwei97910.github.io/blob/main/assets/json/hw10_2.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/yuwei97910/yuwei97910.github.io/blob/main/python_notebooks/group50-assignment10.ipynb" text="The Analysis" %}
</div>
```

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/yuwei97910/yuwei97910.github.io/blob/main/assets/json/hw10_2.json" text="The Data" %}
</div>


<div class="right">
{% include elements/button.html link="https://github.com/yuwei97910/yuwei97910.github.io/blob/main/python_notebooks/group50-assignment10.ipynb" text="The Analysis" %}
</div>

