# NYC taxi trip analysis with PowerBI
This repository contains the analysis and visualization of NYC Yellow taxi trip data from January of 2022. PowerBI was used to build the dashboard of visualizations. 

## Data
Data was downloaded from https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page. Yellow taxi trips from January 2022 was selected. The downloaded parquet file format was converted to CSV format using the Python library Pandas as follows:

```
import pandas
df = pandas.read_parquet("/path_to_data/yellow_tripdata_2022-01.parquet")
df.to_csv("/path_to_output/yellow_tripdata_2022-01.csv",header=True)
```

## Visualization and Analysis with PowerBI
Open the .pbix file [Power BI Desktop file](https://drive.google.com/file/d/1N0mbuyTMNuO8yA0uhrjLj4dRMOisYK_X/view?usp=sharing) in PowerBI to view the dashboard.

Dashboard built with PowerBI has the following components. 

1. KPIs for Total Distance, Total Amount, Average of Trip Distance. 


   In the analysis using card visualization, we can see that the trip distance is 13.24 million miles and generated amount is 47.23 million dollars.
   
   
2. Trip distance by pickup day of week. 


    By checking the trip distance by day data, we can see that Saturday has the highest distance travelled and Wednesday has the lowest.
    
3. Total amount and trip distance by drop off zone.


    From this visual we can see that most of the passengers travel to Upper east side of New York.
    
    
 4. Borough statistics by day of week. 
 
 
    Here we can see that Monday is the busiest day of the week in all boroughs (based on number of trips). 
    
  5. Passenger count by pickup location. 
  
  
     In this donut visual, we can observe that taxis picked up maximum number of passengers from Manhattan. 
     
  6. Amount by payment type. 
     
     
     Maximum number of passengers paid using Credit card.
     
     
 Note that visualizations can be localized to a specific borough and for selected days of the month.

