# WeRateDogs

## Dataset Overview

The dataset contains data from the WeRateDogs Twitter account, including data on tweets, dog ratings, dog breed predictions, and retweets and favorites. The dataset was obtained through various methods, including manual download of individual tweet data and programmatic scraping of data using the Twitter API.

## Data Wrangling Process

The data wrangling process involved several steps, including data gathering, data assessment, and data cleaning. The data was initially assessed for quality and tidiness issues, including missing values, incorrect data types, and duplicated data. The data was then cleaned using a variety of techniques, including dropping unnecessary columns, merging data from different sources, and correcting data inconsistencies.

## Gathering Process

During the data collection phase, I imported the requisite libraries for the data wrangling process. The ‘twitter_arc’ table was obtained and imported into pandas’ data frame using the read function. The ‘images_pred’ table was acquired via the ‘requests’ module, while the final table as a json file that I transformed into a data frame consisting solely of the id, ‘retweet_count’, and ‘favorite_count’ columns.

## Assesing Process

This process consisted in two steps: a visual assessment using a simple code. During this phase, I identified a number of quality and tidiness issues including the need toextract information from certain columns, splits columns, merge columns, delete
columns and handle missing values.

The following step was a programmatic assessment, where I used different pandas’ methods. In this stage, I had more extensive access to the data and was able to identify 
further issues that needed to be addressed during the cleaning such as :
- Delete duplicate values
- Keep only the tweets with images and remove retweets
- Replace not appropriate names
- Capitalize some columns names
- Join the three tables
- Extract information from some columns.

## Cleaning Process

To efficiently address the issued identified during the assessment process, I made a copy of the original data and applied various techniques. This allowed me to perform the cleaning process without affecting original source.

List of the issues addressed

- Drop unnecessary columns
- Crete a column named dog_stage using the values from the columns (doggo, floofer, pupper, puppo)
- Change the data type for the column timestamp and creating a new column for year.

## Data Wrangling Process Conclusion

Data wrangling process is an essential step in the data analysis process. It involvesidentifying and addressing any issues with the data, such as quality problems, 
inconsistencies, or missing values. This process is important because it ensures that the data is in a usable and reliable format for analysis.Without proper data wrangling, the analysis can be difficult or even impossible, as the results may be distorted and misleading due the presence of errors or inconsistencies in the data,

## Acknowledgments

This data wrangling process was completed as part of the Udacity Data Analyst Nanodegree program. Special thanks to the WeRateDogs Twitter account for providing the original dataset and to the Udacity team, Masterschoo' team and instructors for their support and guidance throughout the data wrangling process.
