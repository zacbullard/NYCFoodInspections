# NYC Restaurant Health Ratings

SQL is used to process health inspection data for every report in NYC. The average score per zipcode is calculated and graphed, so New Yorkers can seek out the cleanest (or dirtiest!) neighborhoods for food in the city...

NYC restaurant ratings can be aquired directly from NYC Dept. of Health & Mental Hygiene throught the following [government website.](
https://data.cityofnewyork.us/Health/DOHMH-New-York-City-Restaurant-Inspection-Results/xx67-kt59/data)

The executible code is within `cleanViolations`, which can be run with sqlite via command line as follows:
```
sqlite3 cleanedData.db < cleanViolations
```
A formatted database file `cleanedData.db` will be created in the execution directory, as well as a zipMeans.csv file for ease of plotting. 

![Plotting courtesy of carto.](https://zacbullard.carto.com/builder/28b37ea2-d77f-11e6-b8e8-0ecd1babdde5/embed?state=%7B%22map%22%3A%7B%22ne%22%3A%5B40.52997988184389%2C-74.27581787109376%5D%2C%22sw%22%3A%5B40.870949302299984%2C-73.4044647216797%5D%2C%22center%22%3A%5B40.700682761880564%2C-73.84014129638673%5D%2C%22zoom%22%3A11%7D%7D) 
