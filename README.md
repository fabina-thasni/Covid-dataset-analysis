# Covid-dataset-analysis

![image](https://github.com/user-attachments/assets/0b3afd58-3010-45a6-b378-76ca8413fb0e)

# INTRODUCTION
### The COVID-19 pandemic, caused by the SARS-CoV-2 virus, has resulted in an unprecedented global health crisis.
### Governments, public health institutions, and researchers have been gathering massive datasets to track the spread of the virus. One such dataset is the ECDC COVID-19 dataset from Kaggle, which provides a comprehensive overview of confirmed cases and deaths from various countries across different dates.
### This dataset includes daily records of confirmed cases and deaths reported globally, along with key geographical identifiers. By analyzing this dataset, we can derive insights about the spread of COVID-19 across different countries and territories, the severity of outbreaks, and possible trends or correlations.

# OBJECTIVE

### The goal of this project is to:
### * Analyze the daily trends of COVID-19 cases and deaths.
### * Explore variations in cases and deaths across different countries and regions.

# ECDC_COVID_19:DATASET DESCRIPTION

* dateRep: The date of the reported data

* day: The day of the report (integer, e.g., 1-31).

* month: The month of the report (integer, e.g., 1-12).

* year: The year of the report (integer, e.g., 2020).

* cases: The number of new confirmed cases reported on this date.

* deaths: The number of new deaths reported on this date.

* countriesAndTerritories: The name of the country or territory to which the data belongs.

* geoId: A short geographical identifier (code) for the country or territory.

* countryterritoryCode

## Information of the Dataset

* Columns = 10
* Rows = 9513
* Data types
* float -1
* integer - 5
* object - 4
* Occur Null values
* geoId - 25
* countryterritoryCode - 189
* popData2018 - 143
* No duplicate values
  
## Questions :
* ## filter&sort:
* filter the dataset to include only rows where the countriesandterritories column is either united_states_of_america or india?
* filter the dataframe to include only the rows where the month column is either january or february
* select the rows where geoid is not in a list of excluded codes (excluded_codes=['US','IN','BR'])?
* Filter rows where the countriesAndTerritories column contains 'Germany','France','Italy'.
* Filter out rows where the countriesAndTerritories column not contains 'Germany','France','Italy'.
* extract geoid HR,CU,CW,CY -- reindex,year wise indexing
* extract countries and territory code = GBR, KNA, NLD, PRT --set index in day_name base
* filter the rows where cases>1000 and deaths>500
* set_index is month_name and sort in descending
* extract countriesAndTerritories are 'India','United_Kingdom'  and reindexing with month
* ## pivot()
* create a pivot table in Pandas that shows the total number of deaths reported each month for different countries or territories?
* create a pivot table in Pandas that shows the average number of deaths reported each month for different countries or territories?
* create a pivot table in Pandas that shows the total number of deaths reported each year for different countries or territories?
* create a pivot table in Pandas to display the average population data for 2018 across different years for various countries or territories?
* create a pivot table in Pandas that shows the maximum number of COVID-19 cases reported each month for different countries or territories?
* create a pivot table in Pandas to display the total death rate for each geographic region (geoId) across different days of the week?
* What is the maximum number of COVID-19 cases reported on each day of the week for different geographical regions?
* ## melt():
* reshape a DataFrame in Pandas to combine the cases and deaths columns into a single column, while retaining the countriesAndTerritories and dateRep information?
* ## Groupby():
* What is the maximum number of deaths reported in each country or territory?
* What is the minimum number of COVID-19 cases reported in each country or territory?
* calculate the total number of deaths for each country per year using a Pandas DataFrame?
* find the average population data for 2018 for each country using a Pandas DataFrame?
* determine the maximum, minimum, and total population data for 2018 for each country per year using a Pandas DataFrame?
* find the maximum number of cases and the minimum number of deaths for each country per year using a Pandas DataFrame?
* calculate the minimum, maximum, and average number of deaths for each country per year using a Pandas DataFrame?
* calculate the total number of cases for each country using the countryterritoryCode in a Pandas DataFrame?
* determine the highest number of cases recorded for each country using the countriesAndTerritories and countryterritoryCode in a Pandas DataFrame?
* find the minimum, maximum, and average number of cases for each country using the countriesAndTerritories and countryterritoryCode in a Pandas DataFrame?
* ## Apply():
* create a function in Python that adds 5 to the population data from 2018 for each entry in a DataFrame?
* apply a function to each row of a DataFrame to add 5 to the popData2018 column and store the result in a new column?
* ## idxmax():
* Which row in the dataset corresponds to the highest number of deaths, and what are the details of that row?
* Which country or territory has the lowest minimum death count in the dataset?
* Which row in the dataset corresponds to the lowest number of deaths, and what are the details of that row?
* Which month has the highest maximum number of cases recorded across all months in the dataset?
* ##Cut():
* categorize the number of deaths in your dataset into different levels such as 'Low,' 'Medium,' 'High,' and 'Very High'

# OVERALL INSIGHTS

### Case Increase: COVID-19 cases surged from January to April 2020.
### Deaths Trend: Deaths rose but at a slower rate than cases.
### Country Rankings:
* USA had the highest cases (over 400,000).
* Spain and Italy followed with 150,000 - 200,000 cases each.
* Germany, China, and France reported around 100,000 - 150,000 cases.
* Iran, UK, Turkey, and Belgium had fewer cases, with Belgium having the lowest among these top 10.
### Least Affected Areas: Bhutan and Falkland Islands had only 5 cases, while others like Gambia and Burundi had 4 or fewer.
### Peak Period: Cases and deaths peaked in March and April, then declined by December, January, and February.

# Suggestions

* ###  Strengthen Health Systems: Countries with consistently high cases need better healthcare infrastructure to manage ongoing cases and possible future waves.
* ###  Prepare for Surges: Countries that showed rapid spikes in cases should have systems in place for early detection and rapid response to control outbreaks.
* ###  Localized Policies: Countries with high death rates relative to cases may benefit from targeted health interventions, such as prioritizing vaccinations for vulnerable groups.

# Conclusion

### The ECDC COVID-19 dataset reveals significant trends in the global spread of COVID-19. This analysis provides valuable insights into the countries most affected by the pandemic and the periods of peak transmission. By leveraging visualizations, we can better understand these patterns and guide effective response measures. Future analyses could delve into specific variants, government responses, and the impact of vaccinations over time.
