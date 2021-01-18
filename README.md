# Coursera_Capstone
This is IBM data science Capstone Project 
# Cities' analysis by Venue Ratings.

A description of the problem and a discussion of the background. (15 marks)
A description of the data and how it will be used to solve the problem. (15 marks)
## 1. Introduction to the business problem.
We are a family of three (husband, wife, three y.o. kid) from Torronto planning to move to Europe. Occasionally we have got three job offers: at London (UK), Amsterdam (Netherlands), and Paris (France) and need to decide which city to choose for a living. For now, each city looks equally attractive to us: expecting salary, way of living, language, climate, culture, education, medicine - all these ascpects are comparable to us across these three places and does not help us to make the right decision. The only thing that helps to decide where to move - is its downtown's infrastructure: number of interesting velues (sights, restaurants, children activities, sport centers) that makes our life comfortable and full. The Foursquare data will help us to identify all these places and make the final decision by comparing the results for all three cities.  
 
## 2. Data

We will explore only 3-5 downtown neighbourhoods for each city. The reason for such limitation is:
(a) all companies that made job offers to us are located at the very center of each city;
(b) we are not interested to spend out time/money for a commute;
(c) we want to enjoy historical sights walking around the places concentrated at the downtown.

To get those neighbourhoods (incl. longitide/latitude) we manually have to gether data for:
1. London:
   
2. Amtserdam:
Top boroughs are taken from Trip advisor: https://www.tripadvisor.com/NeighborhoodList-g188590-Amsterdam_North_Holland_Province.html#MAPVIEW
Selected neighbourhood for each borough is taken from postcode site: https://postcode.site/noord-holland/municipality/amsterdam/district/grachtengordel-west
Longitude/latitude for each neighborhood is taken from gogle.maps i.e. https://www.google.com/maps/place/Grachtengordel,+Amsterdam,+Netherlands/@52.3706393,4.8845172,16z/data=!4m5!3m4!1s0x47c609c174cc38ed:0xa9bdbf3f1ac855f9!8m2!3d52.3655774!4d4.8893609


3. Paris:
Top neighbourhoods are taken from: https://www.parisinsidersguide.com/paris-neighborhoods.html
Longitude/Latitude of each neighbourhood is taken from google.maps i.e. https://www.google.com/maps/place/Creperie+and+Kiosk/@48.8543865,2.2912227,15z/data=!4m13!1m7!3m6!1s0x47e6701f7e8337b5:0xa2cb58dd28914524!2sEiffel+Tower,+Paris,+France!3b1!8m2!3d48.8560934!4d2.2930458!3m4!1s0x47e67021d1798475:0xb0cabfbe65e34c5e!8m2!3d48.8544282!4d2.2999573
 
To get top venues for each neighbourhood of the city, we will use Foursquare datawhich will include places of interest, its location, and venue category for each selected neighbourhood which then will be used to rate each category based on our interest, count a rating of each neighborhood and make a final decision.  

## 3. Methodology
## 4. Results
## 5. Conclusion
