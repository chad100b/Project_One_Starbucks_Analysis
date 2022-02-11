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

## Questions for Analysis

1. Is there a correlation between the total number of stores within a city and the
    city's annual average income?
2. Is there a correlation between the total number of stores within a city and the city's population?
3. Are there underserved or overserved cities based on standard deviation from a mean?


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
## Project One Conclusions

1. Is there a correlation between the total number of stores within a city and the
    city's annual average income?
    > We did not see much, if any, coorelation between the number of coffee stores in a given city and the average annual income of that city. The scatter plot shows a similar view at income averages at $45,000/annually as to a city with an average income of $100,000/annually or higher.
2. Is there a correlation between the total number of stores within a city and the city's population?
    > We can see coorelation in the number of stores witin a given city and the population of that city. The scatter plot shows a linear upward trend as population increases, the number of stores increases. This can also be seen from the analysis around the average population count for one store. It is very consistant for most areas.
3. Are there underserved or overserved cities based on standard deviation from a mean?
    > We can derrive a list of good candidate cities to look at for expansion based on those cities that had population averages, per a single coffee shop, well above one standard deviation. We found about 125 cities to investigate and determine if additional stores could be opened.
