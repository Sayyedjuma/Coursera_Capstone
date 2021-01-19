# Coursera_Capstone
This is IBM data science Capstone Project 
# Cities' analysis by Venue Ratings.


## 1. Introduction to the business problem.
We are a family of three (husband, wife, three y.o. kid) from Torronto planning to move to Europe. Occasionally we have got three job offers: at London (UK), Amsterdam (Netherlands), and Paris (France) and need to decide which city to choose for a living. For now, each city looks equally attractive to us: expecting salary, way of living, language, climate, culture, education, medicine - all these ascpects are comparable to us across these three places and does not help us to make the right decision. The only thing that helps to decide where to move - is its downtown's infrastructure: number of interesting velues (sights, restaurants, children activities, sport centers) that makes our life comfortable and full. The Foursquare data will help us to identify all these places and make the final decision by comparing the results for all three cities.  

All these three cities are being very attractive for young well-educated STEM ex-pats who want to immigrate to Europe and the Data Science project is ment to help that group of people in making the right choice. 
 
## 2. Data

We will explore only 3-5 downtown neighbourhoods for each city. The reason for such limitation is:
(a) all companies that made job offers to us are located at the very center of each city;
(b) we are not interested to spend out time/money for a commute;
(c) we want to enjoy historical sights walking around the places concentrated at the downtown.

To get those neighbourhoods (incl. longitide/latitude) we manually have to gether data for:

1. London:
Top boroughs are taken around  Buckingham Palace which is the location of the potential office in London. 
Longitude/latitude is taken from google.maps i.e. https://www.google.com/maps/place/Carnaby,+London,+UK/@51.5132335,-0.139567,18z/data=!3m1!4b1!4m13!1m7!3m6!1s0x47d8a00baf21de75:0x52963a5addd52a99!2sLondon,+UK!3b1!8m2!3d51.5073509!4d-0.1277583!3m4!1s0x487604d51a524419:0x1f4787f88a9cfcb0!8m2!3d51.513283!4d-0.1383859 

2. Amtserdam:
Top boroughs are taken from Trip advisor: https://www.tripadvisor.com/NeighborhoodList-g188590-Amsterdam_North_Holland_Province.html#MAPVIEW
Selected neighbourhood for each borough is taken from postcode site: https://postcode.site/noord-holland/municipality/amsterdam/district/grachtengordel-west
Longitude/latitude for each neighborhood is taken from gogle.maps i.e. https://www.google.com/maps/place/Grachtengordel,+Amsterdam,+Netherlands/@52.3706393,4.8845172,16z/data=!4m5!3m4!1s0x47c609c174cc38ed:0xa9bdbf3f1ac855f9!8m2!3d52.3655774!4d4.8893609


3. Paris:
Top neighbourhoods are taken from: https://www.parisinsidersguide.com/paris-neighborhoods.html
Longitude/Latitude of each neighbourhood is taken from google.maps i.e. https://www.google.com/maps/place/Creperie+and+Kiosk/@48.8543865,2.2912227,15z/data=!4m13!1m7!3m6!1s0x47e6701f7e8337b5:0xa2cb58dd28914524!2sEiffel+Tower,+Paris,+France!3b1!8m2!3d48.8560934!4d2.2930458!3m4!1s0x47e67021d1798475:0xb0cabfbe65e34c5e!8m2!3d48.8544282!4d2.2999573


To get top venues for each neighbourhood of the city, we will use Foursquare datawhich will include places of interest, its location, and venue category for each selected neighbourhood which then will be used to rate each category based on our interest, count a rating of each neighborhood and make a final decision. 

For the visualisation we will use json files for each city that displayed neighbourhood boundaries; 
for London: https://data.london.gov.uk/dataset/statistical-gis-boundary-files-london?resource=9ba8c833-6370-4b11-abdc-314aa020d5e0
for Amsterdam: http://insideairbnb.com/get-the-data.html
for Paris: https://github.com/natzar/European-Neighborhoods-Json-Coords

## 3. Methodology
 We will use cluster analysis to pick up the most attractive neigbourhood in each of three cities. Then to decide which city is better wi will use venue's ranking approach. To do that we take all venues categories from the Foursquare and manually ranking them based on our preferences from 1 to 10 i.e. category "bank" is assigned with rank "3" as we do not use bank offices often while "coffee-shop" will have a rank "7" as we like coffee etc. That city whose neighbourhood will get the highest score will be selected for a living.


