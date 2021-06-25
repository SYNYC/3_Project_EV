# Charging Away From Climate Change

Sabrina Yang


## Abstract

The purpose of this project is to help [Volta Charging](https://voltacharging.com) expand by choosing the optimal locations to place EV charging stations in New York, while taking into account its unique business model and objectives. The client, Volta Charging, has a business model that involves charging an advertising company for ads on its charging stations. This in turn allows EV owners to charge their cars for free and for real estate landlords to have stations for free. A company like this is uniquely positioned to improve climate change, beyond what its competitors can offer. This project will benefit Volta by helping them to understand which counties in New York are most favorable for the construction of new stations. Some of the variables analyzed to determine location favorability include EV ownership, EV sales, population density, sales tax per capita, and daily traffic. Using EV sales data in particular, I was able to forecast future EV sales and thus future charging station demand for the top counties. By determining the top counties, Volta would be able to construct new stations in locations that would maximize customer usage and profitability margin, both of which are key measures of success for the business.



## Design
The project’s goal is to help Volta to determine the counties in New York state that would be the optimal locations to build new charging stations. As such, the choice of variables and data sets to analyze are critical to the success of the project. The variables were chosen based on their likelihood to impact both customer usage and overall profitability for Volta. The variables chosen were EV ownership, EV sales, population density, sales tax per capita, daily traffic, and number of EVs per station. Once data was collected, the next step involved ranking the counties on each of the variables, from best to worst. Some variables are likely more important than others and so a weighted rank was calculated for each county, incorporating all variables. Data and rankings were further analyzed using various charts and graphs, that would glean additional insights. The last step involved predicting future forecasted station demand using EV sales in each county.
  

## Data

The datasets are gathered from [NYS Government Data](https://data.ny.gov) from 6 main excel sheets. The time period of the data is 1 year (2020). However, for forecasting, the dataset for EV sales included a time period of 4 years, from 2017 to 2020. The reason for this is the use 4 year historical data to project EV sales into the future.

0. NYS Zipcode County
1. [Existing EV Charging Stations](https://data.ny.gov/Energy-Environment/Electric-Vehicle-Charging-Stations-in-New-York/7rrd-248n)
2. EV Ownerships
	a. [EV Ownerships by County](https://data.ny.gov/Transportation/Electric-Vehicles-per-County/uu25-czyc)
	b. [EV Number of Registration/Ownerships by Year](https://www.nyserda.ny.gov/All-Programs/Programs/ChargeNY/Support-Electric/Map-of-EV-Registrations)
			
3. [Sales Tax per County](https://data.ny.gov/Government-Finance/State-and-Local-Sales-Tax-Distributions-Beginning-/5g2s-tnb7)
			
4. [Annual Population Density per County](https://data.ny.gov/Government-Finance/Annual-Population-Estimates-for-New-York-State-and/krt9-ym2k)
5. [Annual Average Daily Traffic](https://data.ny.gov/Transportation/Annual-Average-Daily-Traffic-AADT-Beginning-1977/6amx-2pbv)
6. [EV Drive Clean Rebate data](https://data.ny.gov/Energy-Environment/NYSERDA-Electric-Vehicle-Drive-Clean-Rebate-Data-B/thd2-fu8y)
				


## Methodology
*Data Collection*

1. Gathered data from the NYS Government Data by downloading csv. files and consolidating into a single excel file

*Data Manipulation*

2.	Converted zip codes to counties using vlookup functions, as certain datasets don’t have records by county
3.	Calculated combination variables (ie., Number of EVs per Station and Sales Tax per Capita)
4.	Used pivot tables to manipulate data by counties and by time period

*Data Visualization*

5.	Developed various bar charts, line charts, and visual maps incorporating data/variables

*Ranking Calculation*

6.	Ranked each county by favorability according to the 6 variables/datasets
7.	Applied a weighting for each variable and calculated the overall/final rank for each county
8.	Organized the counties from best to worst using index-match function

*Forecasting and Projections*

9.	Calculated the compound annual growth rate for EV sales from 2017 to 2020 by county
10.	Forecasted charging station demand per county by assuming that 1 station is required to support 10 EVs



## Tools

Excel
- Pivot tables
- Vlookup
- Index-match function
- Bar graphs
- Line graphs
- Map visualization tool
- Sort and filter tool

Tableau
- Density maps
- Plotting
- Dot charts


## Summary
The results showed that Suffolk County was the best county based on the variables/datasets analyzed. It consistently scored in the top rankings for each dimension. Nassau County, Queen’s County, King’s County and Bronx County were the next 4 best locations respectively. These results were consistent with the current locations chosen by Volta’s competitors to place their charging stations. Forecasting demand for charging stations by county was also consistent with the ranking approach.


<img src="https://github.com/SYNYC/3_Project_EV/blob/main/charts/Final_Ranking_new.png" width = "950" height = "450">










