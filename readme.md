# Ford GoBike System Data
## by Alex Kim

## Preliminary Wrangling

## Dataset

> This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area.


## Summary of Findings

### What is the structure of your dataset?

> There are 16 columns and 2,383,421 rows in the merged data file for 2017 and 2018 data for bike rental information. There are only 5,404 unique bike_ids in the dataset. There are a couple of categories for user_type and member_gender

### What is/are the main feature(s) of interest in your dataset?

> The main features I'm interested in are start time and end time to calculate when the most trips were taken, duration to calculate how long a trip takes, and whether or not subscribers versus customers make a difference.

### What features in the dataset do you think will help support your investigation into your feature(s) of interest?

> Start time, end time, duration, and user type.

### Discuss the distribution(s) of your variable(s) of interest. Were there any unusual points? Did you need to perform any transformations?

> I transformed the duration in seconds to a logarithmic scale as there was a large distribution from low to high numbers making it difficult to read the graph. By transforming it, I was able to easily depict how long most rentals were being used (between 5 - 18 minutes).

### Of the features you investigated, were there any unusual distributions? Did you perform any operations on the data to tidy, adjust, or change the form of the data? If so, why did you do this?

> I first calculated the age by using the member birth year and then stored it on the dataframe. There seemed to have been ages that were incorrect as there were some ages well beyond 100 years olds (max was 138). Therefore, I filtered out the ages that were over 90 as it seemed highly unlikely that they would be renting these bicycles.


## Key Insights for Presentation

### Talk about some of the relationships you observed in this part of the investigation. How did the feature(s) of interest vary with other features in the dataset?

> Customers are taking longer rides than subscribers but subscribers are taking a lot more rides. The peak months for both customers and subscribers are in September and October.

### Did you observe any interesting relationships between the other features (not the main feature(s) of interest)?

> Subscription growth year over year has increased substantially. Where customer count has stayed relactively the same year over year.

### Talk about some of the relationships you observed in this part of the investigation. Were there features that strengthened each other in terms of looking at your feature(s) of interest?

> Longest rides came from customers and seemed to be more centralized during summer months when it gets really hot. 26-35 year olds used the bikes more than any other age group. There was a significant drop off of rides taken after October for all age groups. Based on the pointplot, no matter what the age group, all of the subscribers seemed to be taking shorter rides. The younger age groups only for customers took longer rides.

### Were there any interesting or surprising interactions between features?

> The subscriber duration seemed pretty consistent throughout the year with slightly higher numbers during the summer. The 36-49 age group had more rides than the 18-25 year old age group. The duration of the people over 50 years old were amongst the highest out of all age groups. 
