# Tied-agents-visualization
Geographical visualization of Tied agents according to the Capital Market Undertakings Act in the Czech Republic

### What's the problem
It is quite difficult to present the layout of the distribution network of Tied agents. Mostly it is processed by a table or column chart aggregated by region where important informaton are missed either in the "big picture" or detail

### The idea
There are many posibilities how to solve the problem mentioned above nowadays. One of the options is to present the data on map that can be zoomed in or out. In addition the chart can be animated by time or distributor.
### The architecture
As programming language Python has been chosen. Source for the list of active Tied agents in Czech Republic is the [ČNB (Czech National Bank)](https://www.cnb.cz/cs/dohled-financni-trh/seznamy/Otevrena-data/). For geocoding purposes [Nominatim](https://nominatim.openstreetmap.org/) is used.
Data manipulation is provided by [Pandas](https://pandas.pydata.org/) and [Geopandas](https://geopandas.org/). Finally, plotting the chart is processed by [Plotly](https://plotly.com/).
### Hierarchy
The directories are organized into following sections:
- scripts: here is a Python (Jupyter Notebook) script that converts address of a particular Tied Agent into geographical coordinates. As search (geocoding) engine is used Nominatim. For more information visit directly [Nominatim](https://nominatim.openstreetmap.org/ui/about.html).
- samples: here are located sample files for geocoding as well as for generating the density heatmap chart as well as final result (density heatmap chart in html)
- src: in this folder are located the source files for geocoding and density heatmap chart
