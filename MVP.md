# MVP
##### Sabrina Yang


The goal of this project was to create a model that predicted and identified the best locations to place the future EV Charging Stations for Volta. 
I did EDA and data visualization on the datasets that I have collected from New York State.
Below are the results for each dataset and its own variables that will be considered in the ranking model toward the target as stations site selection.

## Data Visualization

### 0. NYS County Base Map

There's 63 counties in New York State.

<img src="https://github.com/SYNYC/3_Project_EV/blob/main/charts/New_York_State_Counties_Map.png" width = "650" height = "600">  



### 1. NYS EV Charging Stations 
I colored the existng stations by different EV networks such as ChargePoint, Telsa, Blink, etc. The map shows the cluster are mainly in New York County and followed by Suffolk County, and the rest spread out the entire state. It also shows that our client Volta (_dark purple_) currently owns 4 stations which are located in New York County and Suffolak County as well, so we are going to help them to expand. 

As our expanding strategy, we also prefer to place new stations away from ones that already exist to balance the supply and demand.

<img src="https://github.com/SYNYC/3_Project_EV/blob/main/charts/Tableau_NYS%20EV%20Charing%20Stations.png" width = "1200" height = "600">



### 2. EV Ownerships
#### a. EV Ownerships by County

From this density map, we can spot that the following counties have the highest amount of EV owners: Suffolk, Nassau, Westchester, New York(Queens and Kings), Monroe and Erie. 

<img src="https://github.com/SYNYC/3_Project_EV/blob/main/charts/NYS_EV_Ownership_Density_byCounty.png" width = "750" height = "450">


#### b. EV Number of Ownerships/Users Growth by Year

This Line chart represents the number of new EV owners from 2016 to 2019. We can see it increases over time and peaked during the end of 2018, however the number comes down in 2019 and I assume one of the reasons might be the obstacle that EV users can't find the charging stations as easy as they thought.


<img src="https://github.com/SYNYC/3_Project_EV/blob/main/charts/EV_Number_of_Users_Growth_byYear.png" width = "600" height = "450">


### 3. Sales Tax per County & 4. Popular Density per County
To help us undestanding the customers spending behavior in each County, I took the number of Sales Tax divided by Population for each County to show the overall concept of consumer demographocs.
New York and Suffolk are the top spending customers counties amongst all.

<img src="https://github.com/SYNYC/3_Project_EV/blob/main/charts/SalesTax_PerCapita.png" width = "750" height = "450">


### 5. Annual Average Daily Traffic

To visual the traffic volume and density of the high traffic area in NYS, I made two charts as below 

- AADT Volume Bar Chart
 <img src="https://github.com/SYNYC/3_Project_EV/blob/main/charts/AADT.png" width = "750" height = "450">


- AADT Volume Density Map 
<img src="https://github.com/SYNYC/3_Project_EV/blob/main/charts/AADT_map.png" width = "750" height = "450">



## Ranking

The system is taking the following steps for ranking:

1. **Each Variable Ranking**: For each variable, each county has a number to present its situation. According to these numbers, We ranked all counties from 1 to 63 within its own catergory. 
     
		- Population: more population, higher ranking
		- Sales Tax per Capita: more dollar amount, higher ranking
		- Total EV Owners: more EV owners, higher ranking
		- Number of Stations: less stations, higher ranking (less competitive)
		- EVs per Station Count: higher number, higher ranking (high demand to low supply) 


2. **Weighted Ranking**: The weighted measures is taken by the proportion of Population(25%), Sales Tax per Capita(20%), Total EV Owners(30%), Number of EV per Station(25%).

3. **Final Ranking**: Ranking based on Weighted Ranked data. Here we show the top counties for the overall score as below:

<img src="https://github.com/SYNYC/3_Project_EV/blob/main/charts/Final_Ranking.png" width = "850" height = "450">




