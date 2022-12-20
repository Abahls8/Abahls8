## Seattle Data
#### Alex Bahls -- Command Line GIS

This map shows parking data in Seattle for a select week in October (October 11 - October 17, 2022). Seattle has a dynamic pricing scheme where the price of parking depends in part on the expected demand for parking on that block and so the price of parking on each block varies.  The datasets are prepared by Seattle's Department of Transportation and are updated each day, though only a week of data is hosted at a time due to the size of the datasets. The data has, for each parking transaction, the time, location (with x,y coordinates), amount paid, duration paid for, and method of payment. The data quality was quite high, though there were some issues, specifically rows that had a negative parking duration which I had to remove. 

<iframe src="seattle_parking_final_2.html" height="500" width="95%"></iframe> 

The next map shows the total revenue for each block and how people typically paid for the parking. The size each point represents the amount of revenue, with larger circles representing more revenue for the city. Points in orange were blocks where at least 75% of transactions were paid for via phone application, and points in blue were where less than 75% transaction were paid for via phone. I chose 75% as a cut-off as phone applications were by far the most common method of paying for parking.

<iframe src="Parking_map_1_Ill_map.png" height="500" width="95%"></iframe> 

The last map shows the total parking revenue by census tract. Lighter tracts bring in more parking revenue for the city. This map was created by doing a spatial join to determine which meters were in which census tracts and then aggregating the total revenue for each meter up to the census tract level. 

<iframe src="Parking_map_2.png" height="500" width="95%"></iframe> 
