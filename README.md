# PROJECT: Starbucks Locations Analysis

## Team:
- Chad Burford
- Erik McFarlane
- Diego Torres

## GOALS:

1. Find US data for all Starbucks locations
2. Find US census information (total population, population density, income) by city
3. Find Min/Max/Avg/StD. for Starbucks locations versus census information
4. Based on #3 determine top underserved and overserved locations on a per capita/income basis

## Code Approach:

<ol>
  <li>Import relevant libraries</li>
  <li>Import datasets</li>
  <ol>
    <li>Starbucks dataset <i>('Data_Files/starbucks_locations.csv.txt')</i></li>
      <ul><li>Convert dataset into a Dataframe</li>
          <li>Sanitize dataset (drop unnecessary columns)</li>
          <li>Filter unnecessary values</li>
          <li>Make relevant groupings in order to: get number of stores for each city and get the cities' Latitude/Longitude</li>
          <li>Merge grouby results into Dataframe that will be merged with other datasets</li>
      </ul>
    <li> U.S. income information by city <i>('Data_Files/kaggle_income.csv')</i></li>
      <ul><li>Convert dataset into a Dataframe</li>
          <li>Sanitize dataset (drop unnecessary columns)</li>
          <li>Filter unnecessary values</li>
          <li>Homogenize column names to merge with Starbucks dataframe</li>
          <li>Merge with Starbucks dataframe</li>
      </ul>
    <li> U.S. income population by city <i>('Data_Files/us population with cordinates.csv.txt')</i></li>
      <ul><li>Convert dataset into a Dataframe</li>
          <li>Sanitize dataset (drop unnecessary columns)</li>
          <li>Filter unnecessary values</li>
          <li>Homogenize column names to merge with combined Income/Starbucks dataframe</li>
          <li>Merge grouby results into final combined Dataframe</li>
      </ul>    
  </ol>    
  <li>Analysis</li>
  <ol>
    <li>Create scatter plots  <img title="Scatter Plot" alt="scatter plot" src="https://github.com/pentius00/Starbucks_analysis/blob/main/populaton_store_count_chart.png">
    <li>Create map "heat" plots <img title="Starbucks Heat Map" alt="Heat Map" src="https://github.com/pentius00/Starbucks_analysis/blob/main/map_locations_data.png">
    <li>Create standard deviation plot</li>  <img title="Standard Deviation Plot" alt="STD plot" src="https://github.com/pentius00/Starbucks_analysis/blob/main/store_count_std.png">
    <li>Combine plots into an interactive dashboard</li>
    <ol>
      <li>Number of Starbucks per city per population</li>
      <li>Avg income per starbucks per city</li>
      <li>U.S. income information by city</li>
      <li>Chart/Scatter plot of locations vs. #3 (will determine which cities have too many or too few Starbucks</li>
    </ol>
  </ol> 
</ol>  
