# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The project goal is to using data retrieved from FourSquare and Yelp in a specific city to analyze and build a model about the relationship of number of avaible bikes at a location with POIs nearby

## Process
### Retrieve the data from city bikes
Using the URL `http://api.citybik.es/v2/networks` to find the data at a location of choice. Here I selected Siena, Italy to get the data
The output is city_bikes.csv under `data` folder
### Retrieve the data from Foursquare
Using the URL `https://api.foursquare.com/v3/places/search` and `https://api.yelp.com/v3/businesses/search` to find the POIs at a location of choice. 


The output is `foursquare_yelp.csv` under data folder

### Store the data in database
Connect to the `sqlite` and store the data in the table `pois` in the database

### Retrieve data from database
Connect to the `sqlite` and get the data in the table `pois` from the database

### Build the linear regression model
Clean the data retrieved from database
Build the linear regresion model for the dependant variable `free_bikes` to others
## Results
The data from Yelp provide more POIs than Foursquare
The model shows that there is a statistically significant of latitude and logitude to the number of bikes at a location

## Challenges 
How to define the independant variables which has a correlation to the number of bikes

## Future Goals
(what would you do if you had more time?)
Try to see if I can apply the Logistic regression model / Classification model with the data from APIs