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
  * This section calculates the average number of housing units per year and visualizes the results using a bar chart.

2. Calculate and plot the average prices per square foot.

3. Compare the average prices by neighborhood.

4. Build an interactive neighborhood map.

5. Compose your data story.




## Results

1. What’s the overall trend in housing units over the period that you’re analyzing?
*Calculate and Plot the Average Sale Prices per Square Foot
For this part of the assignment, use numerical and visual aggregation to calculate the average prices per square foot, and then visualize the results as a bar chart. To do so, complete the following steps:

Group the data by year, and then average the results. What’s the lowest gross rent that’s reported for the years that the DataFrame includes?

Create a new DataFrame named prices_square_foot_by_year by filtering out the “housing_units” column. The new DataFrame should include the averages per year for only the sale price per square foot and the gross rent.

Use hvPlot to plot the prices_square_foot_by_year DataFrame as a line plot.

HINT
Style and format the line plot to ensure a professionally styled visualization.

Note that your resulting plot should appear similar to the following image:

6-4-avg-sale-px-sq-foot-gross-rent.png

Use both the prices_square_foot_by_year DataFrame and interactive plots to answer the following questions:

Did any year experience a drop in the average sale price per square foot compared to the previous year?

If so, did the gross rent increase or decrease during that year?

Compare the Average Sale Prices by Neighborhood
For this part of the assignment, use interactive visualizations and widgets to explore the average sale price per square foot by neighborhood. To do so, complete the following steps:

Create a new DataFrame that groups the original DataFrame by year and neighborhood. Aggregate the results by the mean of the groups.

Filter out the “housing_units” column to create a DataFrame that includes only the sale_price_sqr_foot and gross_rent averages per year.

Create an interactive line plot with hvPlot that visualizes both sale_price_sqr_foot and gross_rent. Set the x-axis parameter to the year (x="year"). Use the groupby parameter to create an interactive widget for neighborhood.

Style and format the line plot to ensure a professionally styled visualization.

Note that your resulting plot should appear similar to the following image:

6-4-pricing-info-by-neighborhood.png

Use the interactive visualization to answer the following question:

For the Anza Vista neighborhood, is the average sale price per square foot for 2016 more or less than the price that’s listed for 2012?
Build an Interactive Neighborhood Map
For this part of the assignment, explore the geospatial relationships in the data by using interactive visualizations with hvPlot and GeoViews. To build your map, use the sfo_data_df DataFrame (created during the initial import), which includes the neighborhood location data with the average prices. To do all this, complete the following steps:

Read the neighborhood_coordinates.csv file from the Resources folder into the notebook, and create a DataFrame named neighborhood_locations_df. Be sure to set the index_col of the DataFrame as “Neighborhood”.

Using the original sfo_data_df Dataframe, create a DataFrame named all_neighborhood_info_df that groups the data by neighborhood. Aggregate the results by the mean of the group.

Review the two code cells that concatenate the neighborhood_locations_df DataFrame with the all_neighborhood_info_df DataFrame. Note that the first cell uses the Pandas concat functionLinks to an external site. to create a DataFrame named all_neighborhoods_df. The second cell cleans the data and sets the “Neighborhood” column. Be sure to run these cells to create the all_neighborhoods_df DataFrame, which you’ll need to create the geospatial visualization.

Using hvPlot with GeoViews enabled, create a points plot for the all_neighborhoods_df DataFrame. Be sure to do the following:

Set the size parameter to “sale_price_sqr_foot”.

Set the color parameter to “gross_rent”.

Set the frame_width parameter to 700.

Set the frame_height parameter to 500.

Include a descriptive title.

Note that your resulting plot should appear similar to the following image:

6-4-geoviews-plot.png

Use the interactive map to answer the following question:

Which neighborhood has the highest gross rent, and which has the highest sale price per square foot?
Compose Your Data Story
Based on the visualizations that you created, answer the following questions:

How does the trend in rental income growth compare to the trend in sales prices? Does this same trend hold true for all the neighborhoods across San Francisco?

What insights can you share with your company about the potential one-click, buy-and-rent strategy that they're pursuing? Do neighborhoods exist that you would suggest for investment, and why?
