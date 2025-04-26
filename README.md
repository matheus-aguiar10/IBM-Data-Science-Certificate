# Data Science Professional Certificate - Final Project: Restaurant Location Analysis in Toronto

This project analyzes data to determine the optimal location and cuisine type (Japanese or Italian) for a new restaurant in Toronto, Ontario, Canada.    

**1. Introduction: Business Problem**
The foodservice market in Toronto is highly competitive.  Opening a new restaurant requires careful analysis to maximize success.  This project aims to provide insights to help stakeholders decide whether to open a Japanese or Italian restaurant and identify the best location within Toronto.  A good location that attracts attention and avoids areas with high competition is crucial.  Locations close to the city center or areas with a large flow of people are preferred.    

**2. Data Acquisition and Analysis**
The analysis is based on data obtained using the Foursquare API.    

**2.1. Data Sources and Factors**
The factors influencing the decision are:

The total number of existing restaurants in a candidate area.    
The number and distance of existing Italian or Japanese restaurants in the neighborhood.    
The distance of a potential restaurant location from the city center or areas with a high flow of people.    
Approximate addresses of candidate area centers were obtained using the Foursquare API.    

**2.2. Data Cleaning and Exploration**
A map of Toronto with neighborhoods was plotted.  Geographical coordinates for Toronto were obtained to facilitate map creation.  Foursquare API was used to get venue data within a 1500-meter radius, filtering for Japanese and Italian restaurants, as well as all other restaurants.  The data, initially in JSON format, was transformed into Pandas data frames for analysis, extracting the venue name, category, latitude, and longitude.    

Maps were generated to visualize the distribution of:

Japanese Restaurants: These show a high concentration downtown, particularly on Dundas Street, and another cluster near the financial district. The competition among Japanese restaurants appears high due to their proximity.    

Italian Restaurants: These are not as evenly distributed as Japanese restaurants, with concentrations downtown and primarily in the financial district area. The distance between Italian restaurants is generally greater, suggesting less direct competition compared to Japanese restaurants. There are also fewer Italian restaurant options overall.    

All other restaurants (excluding Japanese and Italian): The area near the financial district has a very high concentration of other restaurant types, indicating high overall competition in this sector.    

An analysis of the most common restaurant types in Toronto based on 100 venues showed that after general "Restaurants" and "Cafés," Italian and Japanese restaurants are among the most common. Italian restaurants represent 8% of the market, followed by Japanese restaurants at 7%.    

**3. Conclusion**
Based on the analysis of competition, distribution, and popularity:

Cuisine Choice: Opening an Italian restaurant is recommended over a Japanese one.  This is due to less direct competition among Italian restaurants (greater distance between them and fewer options) and the popularity of Italian food in the city.    
Location Choice: Downtown Toronto is the preferred location for a new Italian restaurant.  While the financial district has high weekday traffic, downtown offers more consistent consumption, fewer existing Italian restaurants with larger distances between them, and benefits from tourist flow in addition to residents.    
The final decision based on this report is to open an Italian restaurant in downtown Toronto. 



