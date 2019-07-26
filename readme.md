# Ford GoBike Data  - Exploratory Analysis

GoBike program offers a biking transportation infrastructure to connect the people of the
bay area to numerous locations in SF, East Bay and San Jose. The Ford GoBike infrastructure involves having locations where people can rent bikes at any station and drop them off
at any station. As a result, the consumers never have to pay for an actual bike, deal with
maintenance of a bike, or worry about having a bike being stolen.

The dataset being used in this report is bike share data sourcing from Ford GoBike, formerly known as ”Bay Area Bike Share”. The company publishes system and real-time data based on the ”General Bikeshare Feed Specification”, which allows users to query data via their maintained real-time API

# The Dataset

The dataset being used in this report is bike share data sourcing from Ford GoBike, formerly known as ”Bay Area Bike Share”. The company publishes system and real-time data based on the ”General Bikeshare Feed Specification”, which allows users to query data via their maintained real-time API.


# Data Gathering 

The Data was programmatically downloaded from the the following link https://s3.amazonaws.com/baywheels-data/index.html
that included a CSV file for the year 2017, and zip files for every month till today's date.
# Cleaning Efforts 
The original dataset came with the following infomration(columns):

- bike_id                          
- bike_share_for_all_trip     
- duration_sec                     
- end_station_id               
- end_station_latitude             
- end_station_longitude            
- end_station_name             
- end_time                         
- member_birth_year           
- member_gender               
- rental_access_method       
- start_station_id             
- start_station_latitude           
- start_station_longitude      
- start_station_name           
- start_time                       
- user_type                        

********************
- dropping columns with high amount of missing data
- dropping rows with missing data
- correcting datatype of start_time
- correcting datatype of end_time
- reoganizing columns, taking only columns of interest
- saving the clean dataframe to a csv file on disk

# key insights from the analysis
- majority of the riders are between the age of 25-44
- males have fewer riding durations 
- bikes were used for commuting as the rides were signigicantly less on weekends 
- most of the riders are loyal user ie: subscribers 
