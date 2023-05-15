# San Francisco Housing Market Analysis
# Table of Contents
* [Background](#Background)
* [Instructions](#Instructions)
* [Data](Data)
* [Analysis](#Analysis)
* [Dependencies](#Dependencies)
* [Utilization](#Utilization)

# Background 
* This project analyzes the housing market in San Francisco using housing sales data from 2010 to 2016. The analysis consists of several visualizations to understand the trends and relationships in the data.

# Analysis

1. Calculate and plot the housing units per year.
   * Calculates the average number of housing units per year and visualizes the results using a bar chart.

2. Calculate and plot the average prices per square foot.
   * Calculates the average sale price per square foot by year, filters out the housing_units column, and visualizes the results using an interactive line plot.

3. Compare the average prices by neighborhood.
   * The data is grouped by year and neighborhood, and the mean values are calculated. An interactive line plot is created using hvplot, allowing users to select a neighborhood from a dropdown menu and view the average price per square foot for the selected neighborhood.
  
4. Build an interactive neighborhood map.
   * Combines the neighborhood location data with the average prices to create an interactive map using hvplot and GeoViews. The map displays points for each neighborhood, with the size of the points representing the sale price per square foot and the color representing the gross rent.
  
 # Dependencies
 * Python
 * Pandas
 * hvPlot
 * GeoViews
 * Jupyter Notebook
# Utilization
* Run the analysis via Jupyter Notebook San_francisco_housing_analysis.ipynb and execute the cells in chronological order. 
