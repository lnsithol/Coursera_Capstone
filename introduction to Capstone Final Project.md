
# Capstone Project Requirement

Now that you have been equipped with the skills and the tools to use location data to explore a geographical location, over the course of two weeks, you will have the opportunity to be as creative as you want and come up with an idea to leverage the Foursquare location data to explore or compare neighborhoods or cities of your choice or to come up with a problem that you can use the Foursquare location data to solve. If you cannot think of an idea or a problem, here are some ideas to get you started:

1. In Module 3, we explored New York City and the city of Toronto and segmented and clustered their neighborhoods. Both cities are very diverse and are the financial capitals of their respective countries. One interesting idea would be to compare the neighborhoods of the two cities and determine how similar or dissimilar they are. Is New York City more like Toronto or Paris or some other multicultural city? I will leave it to you to refine this idea.



2. In a city of your choice, if someone is looking to open a restaurant, where would you recommend that they open it? Similarly, if a contractor is trying to start their own business, where would you recommend that they setup their office?


These are just a couple of many ideas and problems that can be solved using location data in addition to other datasets. No matter what you decide to do, make sure to provide sufficient justification of why you think what you want to do or solve is important and why would a client or a group of people be interested in your project.

# 1. Purpose

This report provides the details of my final peer reviewed assignment for the IBM Data Science Professional Certificate Program- Coursera Capstone.

# 2. Introduction

Singapore, an island city-state off southern Malaysia, is a global financial centre with a tropical climate and multicultural population. According to the United Nations World Bank Statistics, the city-state has a total population of 5.61 million in 2017. Accoring to the Housing and Development Board(HDB), 3.25 million people in Singapore live in HDB flats. Public housing also known as HDBs which has a lease of 99 years are managed by the HDB. Due to her small land size, prices of public flats have soared to record levels. As a result, this has led to increase in price of rentals over the years. 

In this report, we will attempt to apply data analysis methodologies to analyse Singapore's Property Market and as well as its correlation to the amneties in its surrounding.
These amnetites can be broken down into:
- Nearby Schools
- Transport Facilities
- Food locations 
- Outdoors and recreation

I will limit the scope of this search as FourSquare API only allows 50 free venue query limit per day when using a free user access


This report is suitable for foreign workers, tourists or property owners who wish to understand about the various town and ameneties within the area.

# 3. Data Acquisition

### Singapore Towns and Median residential rental prices
Property prices, median rent by town and flat type data will be retrieved from Singapore open dataset from https://data.gov.sg/

### Singapore Top Venue Recommendations from FourSquare API
Location information will be parsed from https://www.foursquare.com

I will be using the FourSquare API to explore neighbourhoods in Singapore. The FourSquare explore function will be used to get the most common venue categories in each neighbourhood, and then use this feature to group the neighbourhoods into clusters. The following information are retrieved on the first query: 

- Venue ID
- Venue Name
- Coordinates: Latitude and Longitude
- Category Name

The second query will be performed to retrieve venue ratings for each location identified. 

## 4. Methodology

Singapore Towns List with median residential rent
1. Data cleanup/preprocessing
2. Retrieve Town Coordinates
3. Generate Singapore basemap
4. Retrieving FourSquare places of interest
5. Exploring Neighbourhood in Singapore
6. Data cleanup on duplicates and removing ratings with no ratings
7. Analyse each Singapore town
8. Clustering the towns into clusters
9. Data Visualisation
