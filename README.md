# Charging your way to Climate Change   

# Project Proposal



## Introduction


### Backstory: 

President Biden has declared that he would like to help subsidize the construction of 500k charging stations across the US over the next decade, which would be a huge windfall for companies such as Volta. 

The Biden administration would like to spend $15 billion to increase the national electric-vehicle charging network to half a million stations by 2030. Biden has repeatedly promised that he’ll set the country on course to zero out carbon emissions by 2050. The US could have 35 million EVs by 2030, requiring millions of plugs where the country only has 100,000. Meanwhile, a lack of charging infrastructure is one of the top hurdles to EV ownership.

The Biden administration has not determined how and where charging stations will be built, so private companies that bring solutions to Biden can gain in favor in this new age.

### Client:

**Volta Charging**

Volta is a entrepreneurial charging company with a unique business model, very different from other larger competitors such as ChargePoint or EV Box. 

Volta's business model is centered around advertising partnerships that drive revenue. Similar to how Google and Facebook offer free products/solutions, Volta offers free charging for both vehicle owners and real estate landlords. Volta instead charges large companies for advertising space on their charging station screens (i.e., nestle, nike, monster, etc.). EV owners receive free charging and real estate owners (shopping malls, parking lots etc.) are given free charging stations that  bring higher traffic to their locations.This is in contrast to many of Volta's competitors that require either EV owners or real estate owners to pay for charging.



## Problem

To help Volta Charging expand by choosing the optimal locations to place EV charging stations in New York, while taking into account its unique business model and objectives.


## Data Science Solution path

**WHEN and WHERE**

How to choose the best locations:
	- Use multiple datasets to analyze variables that are important to the choice of EV charging locations
	- Datasets/Variables include:
	
	        0. NYS Zipcode County 
    			- To group the zidcodes into county in order to analyze data based on each County 
		1. Existing EV charging stations
				- Prefer to place new stations away from ones that already exist
		2. EV Ownerships
			a. EV Ownerships by County
				- Areas with higher EV ownership are more likely to use the charging stations as the 
			b. EV Number of Ownerships/Users Growth by Year
				- Helps project the station building plan over the next years, matching supply and demand
		3. Sales Tax per County
				- Includes general retail sales and compensating use tax OR sales tax on a consumer utilities services 
				- To help undestanding the customers spending behavior in each County
		4. Popular Density per County
				- Areas with higher population are more likely to use the charging stations
				- To help undestanding the customers base and potential user amounts in each county
		5. Annual Average Daily Traffic
				- Track the Daily Traffic Volume to determine the high traffic locations/Counties
				


## Impact Hypothesis
Choosing the optimal charging station locations will help the business to develop a competitive advantage and acquire defensible market share from competitors.

By using the prediction model, Volta can identify/prioritize the best locations to place its future EV charging stations. By analyzing various datasets and variables, the company will be able to maximize profits, customer utilization and overall brand awareness.  Additionally, brand partners that advertise through Volta will see higher satisfaction and effectiveness in money spent. This can result in sustainable long-term partnerships and higher levels of customer retention.


## Measures of success

Non-technical metrics: 
1. Customer Usage Growth % :
customer usage measured per station by calculating the number of new customers per period, customer visits per day, and the amount of electricity charged per day. 

2. Profitability Margin % :
measured by the net income margin and EBITDA margin. Although revenue and profit on an absolute basis will increase as charging stations increase, margins will be the key measure of whether the stations increase overall profitability per station.

Technical metrics: 
1. The model will be run daily to monitor the customer usage change of each station, helping to adjust the future location plans. Also, the model will be updated with customer data to allow for continual improvements. 



## Risk and assumptions

1. Undesirable location chosen:
If the wrong choice is made for a charging station location, this could result in lower profitability and customer utilization after the fixed cost has been incurred. In order to mitigate this, as many variables and datasets must be analyzed as possible to increase confidence in location choice
2. Competitors acquire location first:
Once Volta has determined optimal locations, there is a chance that a competitor may  takeover the location first. In order to mitigate this, we must focus on locations that benefit from Volta's competitive edge, which is that real estate landlords will not have to pay for the stations. Certain locations such as shopping malls and movie theatres may be more inclined to go with Volta over a competitor that charges them





## Tools
1. Excel
2. Tableau



## Workflow
1. Data Acquisition  ([NYS Goverment Data](https://data.ny.gov))
2. EDA with excel
3. Tableau for Mapping


## MVP Goal

✨Multiple excel data tables and graphs that  indicate the ranking of each county in New York, based on each dataset/variable that impacts location attractiveness.✨
