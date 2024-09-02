# Covid-dataset-analysis

![image](https://github.com/user-attachments/assets/0b3afd58-3010-45a6-b378-76ca8413fb0e)

CDC_COVID_19:DATASET DESCRIPTION

* dateRep: The date of the reported data

* day: The day of the report (integer, e.g., 1-31).

* month: The month of the report (integer, e.g., 1-12).

* year: The year of the report (integer, e.g., 2020).

* cases: The number of new confirmed cases reported on this date.

* deaths: The number of new deaths reported on this date.

* countriesAndTerritories: The name of the country or territory to which the data belongs.

* geoId: A short geographical identifier (code) for the country or territory.

* countryterritoryCode

Information of the Dataset

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
  
Questions :
* ##filter&sort:
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
* ##pivot()
* create a pivot table in Pandas that shows the total number of deaths reported each month for different countries or territories?
* create a pivot table in Pandas that shows the average number of deaths reported each month for different countries or territories?
* create a pivot table in Pandas that shows the total number of deaths reported each year for different countries or territories?
* create a pivot table in Pandas to display the average population data for 2018 across different years for various countries or territories?
* create a pivot table in Pandas that shows the maximum number of COVID-19 cases reported each month for different countries or territories?
* create a pivot table in Pandas to display the total death rate for each geographic region (geoId) across different days of the week?
* What is the maximum number of COVID-19 cases reported on each day of the week for different geographical regions?
* ##melt():
* reshape a DataFrame in Pandas to combine the cases and deaths columns into a single column, while retaining the countriesAndTerritories and dateRep information?
* ##Groupby():
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
* ##Apply():
* create a function in Python that adds 5 to the population data from 2018 for each entry in a DataFrame?
* apply a function to each row of a DataFrame to add 5 to the popData2018 column and store the result in a new column?
  
