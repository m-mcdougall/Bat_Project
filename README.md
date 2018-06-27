
# Bat Population Data Exploration 
The Bat Population Data Exploration is an exploratory analysis project. 
Data was downloaded from the [Bat Population Data Project](https://my.usgs.gov/bpd/), an ongoing effort by the United States Global Survey (USGS) to provide a central repository and standard for bat population surveying. 

While the BPD contains entries for data including bat captures and weights dating back over 200 years, my initial survey of the data determined that population counts from 1918 - 2018 was the most consistent data, hence my analysis is focused on observing bat populations from 1918 - 2018. By cleaning and visualizing this data, I hope to explore range information for individual species, as well as trends in populations over time.

## Repository Contents
-  Bat Stuff.ipynb: Code used for downloading, cleaning and organizing the BPD
    
-   Bat_Data_1918_to_2018.csv: Output of data wrangling from Bat Stuff.ipynb

## Visualization

To explore bat population patterns, you can use the db_clean Pandas Dataframe and the bats_pop_time() function located in Bat Stuff.ipynb. For example:
```python
#Looking a bat population numbers from 1950 - 1955 in Maryland and California
states_of_interest = ["Maryland","California"]
dates_of_interest = [1950, 1955]
bats_pop_time(df, states_of_interest, dates_of_interest, graph = True)
```


## Future Analyses
This project is an ongoing work in progress. The following are analyses/visualizations that are planned for the future:

- 2D Line Plots of bat populations over time.
- Heatmap of bat population counts projected onto a map of the USA, by state and by county using the Plotly library (choropleth map).
  
