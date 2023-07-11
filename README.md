# San Francisco Housing Market Analysis
# Table of Contents
* [Background](#Background)
* [Instructions](#Instructions)
* [Data](Data)
* [Analysis](#Analysis)
* [Dependencies](#Dependencies)
* [Utilization](#Utilization)

# Background 
* Proptech, the application of technology to real estate markets, is an innovative domain in the fintech industry. This project focuses on analyzing the housing rental market data for San Francisco. The goal is to identify viable investment opportunities for a proptech company that wants to offer an instant, one-click service for people to buy properties and then rent them.

The analysis utilizes data visualization techniques, including aggregation, interactive visualizations, and geospatial analysis, to explore the San Francisco real estate market and identify potential investment opportunities.


# Files
* san_francisco_housing.ipynb: Jupyter notebook containing the analysis of the housing rental market data for San Francisco.
* sfo_neighborhoods_census_data.csv: Dataset file that includes information about housing units, sale price per square foot, and gross rent for various San Francisco neighborhoods.
* neighborhood_coordinates.csv: Dataset file containing latitude and longitude coordinates for each neighborhood, used for geospatial visualizations.

# Instructions
* Download the project files and save them in your working directory.
* Open the Jupyter notebook san_francisco_housing.ipynb.
* Make sure you have the required dependencies installed, including Python, Pandas, hvPlot, and GeoViews.
* Run the notebook cells in chronological order to execute the analysis and generate the visualizations.


# Data 
* The dataset used for this analysis is sfo_neighborhoods_census_data.csv, which includes information about housing units, sale price per square foot, and gross rent for various San Francisco neighborhoods. 

* The neighborhoods_coordinates.csv file contains latitude and longitude coordinates for each neighborhood, which are used for geospatial visualizations.

# Analysis
* Calculate and Plot the Housing Units per Year
* Calculates the number of housing units per year by grouping the data by year and aggregating the results.
* Visualizes the housing units per year as a bar chart using hvPlot.
* Examines the overall trend in housing units over the analyzed period.
  
# Calculate and Plot the Average Sale Prices per Square Foot
* Groups the data by year and averages the results.
* Determines the lowest reported gross rent for the years included in the dataset.
* Creates a new DataFrame with average sale price per square foot and gross rent per year.
* Visualizes the average sale prices per square foot over the years as a line plot using hvPlot.
* Analyzes whether any year experienced a drop in the average sale price per square foot compared to the previous year and examines the corresponding change in gross rent.
# Compare the Average Sale Prices by Neighborhood
* Groups the data by year and neighborhood, and calculates the mean values.
* Filters out the "housing_units" column to create a DataFrame with average sale price per square foot and gross rent per year.
* Creates an interactive line plot using hvPlot to visualize the average sale prices and gross rent per year, with a dropdown menu for selecting neighborhoods.
* Compares the average sale price per square foot for the Anza Vista neighborhood in 2016 and 2012.
# Build an Interactive Neighborhood Map
* Reads the neighborhood coordinates data from the neighborhood_coordinates.csv file and creates a DataFrame.
* Groups the original data by neighborhood and calculates the mean values.
* Combines the neighborhood location data with the average prices to create an interactive map using hvPlot and GeoViews.
* Creates a points plot where the size of the points represents the sale price per square foot and the color represents the gross rent.
* Identifies the neighborhood with the highest gross rent and the one with the highest sale price per square foot.
# Conclusion
Based on the analysis of the San Francisco housing rental market data, the following conclusions can be drawn:

* The overall trend in housing units shows an increase over the analyzed period, indicating potential growth in the real estate market.
* The average sale prices per square foot generally increased over the years, with occasional drops in certain years. During years with drops in sale prices, the gross rent either increased or decreased, depending on the specific year.
* When comparing average sale prices per square foot by neighborhood, the Anza Vista neighborhood had a higher average sale price in 2016 compared to 2012.
* The interactive neighborhood map provides insights into the distribution of sale prices per square foot and gross rent across different neighborhoods. It helps identify neighborhoods with high rental income potential and high sale prices per square foot.

  
Based on the analysis, the proptech company could consider investing in neighborhoods that exhibit high potential for rental income growth and have relatively high sale prices per square foot. The specific neighborhoods could be identified by examining the map visualization and considering factors such as average sale prices, gross rent, and market trends.

Please refer to the Jupyter notebook san_francisco_housing.ipynb for a detailed analysis and visualization of the San Francisco housing rental market data.  
