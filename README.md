# Factors-Influencing-Walkability-A-Comparative-Analysis-Across-US-Combined-Statistical-Areas
Factors Influencing Walkability of US Combined Statistical Areas (CSAs)

## PowerBI Dashboard
Link: https://app.powerbi.com/view?r=eyJrIjoiZGJhMDVjOGMtNzFkYi00ZDJkLWJiMGQtZDE5MTIxNTllMTQ3IiwidCI6IjEwMWRhNTg3LTE4NDMtNGY1Mi04YjhhLTE3YjA2OWM2NmQzMyIsImMiOjJ9

Table of Contents

* [PowerBI Dashboard](#powerbi-dashboard)
* [Motivation](#motivation)
* [Questions](#questions)
* [Normalizing the Data/Methodology](#normalizing-the-datamethodology)
* [Problems and Hurdles](#problems-and-hurdles)
* [Technologies Used](#technologies-used)
* [Sources](#data-sources)
* [Conclusion](#conclusion)

## Motivation:

My motivation behind this project was inspired by my personal experience living in Nashville, where getting around the city feels incredibly car dependent compared to other cities I have visited. This highlighted the stark variation in pedestrian infrastructure across different regions. So, I decided I needed to dig a little deeper to see if I could find factors that are driving walkability in US cities. This project aims to move beyond anecdotal observations to give a more data driven analysis on walkability. I narrowed down the Top 15 and Bottom 15 CSAs for Walkability in the US and looked at many factors from Socioeconomic, Demographic, and Built Environment. The analysis showed that the top factor categories were Built Environment and Socioeconomic. The data is from 2021.

## Questions: 

1.) Which demographic, socioeconomic, and built environment factors correlate with higher walkability scores at the CSA level?

2.)How strongly do commuting behaviors relate to the potential for walkability across CSAs?

3.)How do the top 15 CSAs stack up to the bottom 15 CSAs, which factors have the largest gap between top and bottom?

4.)What are the absolute best walkability CSAs (Small, Medium, Large) and what are the worst? How do they compare with one another?

## Normalizing The Data/Methodology:

Originally the walkability score data was based on Census Block Groups (CBG) the CBG level is the most granular data that the Census collects. Unfortunately this data wasn't avaialable en masse for all of the CBGs I was returning. I decided to go one more level up and see if I could find all of the data for the Core Based Statistical Areas or CBSA. After getting my 30 CBSAs returned the same problem occurred where all of the data wasn't available. I had to normalize the data to be on the Combined Statistical Area (CSA) this level can contain a few counties so it masks neighborhood level variation.

Populations were broken down into 3 distinct categories. Small (<175k population>), Medium (<=500k population), Large (>500k population)

Top and Bottom scoring CSAs were found by finding the nlargest 5 and nsmallest 5 scores for each size category.

Originally went with 25th, 50th, 75th percentile(s) for 

Correlations were all ran using the Spearman method.

## Problems and Hurdles:

My biggest Challenge with this project was Data Granularity. I originally intended to look at the Core-Based-Statistical-Area (CBSA) level which is closer to our definition of what a city is. But, unfortunately the data was not readily available without incredibly time consuming manual cleaning so I went with CSA level data which can contain a few counties - This can and will mask neighborhood-level variation. But, with that being said the CSA level data can still give us a really good idea of where the more walkable and not so walkable cities are located in the US.

## Technologies Used

Python / Pandas - for exploration, correlations, normalizing, aggregations, and joining of the datasets
PowerBI - for creating interactive dashboard
PowerPoint - for introduction of Project
Git - for version control
Excel - cleaned a few things using it that would've been more time consuming using Python.

## Data Sources
To answer the above questions I used the following sources to collect datasets for my analysis

Walkability Index from EPA
https://www.epa.gov/smartgrowth/smart-location-mapping#walkability

DP(Data Profile) DP02-DP05 Census Data
    https://data.census.gov/table/ACSDP5Y2022.DP02
    https://data.census.gov/table/ACSDP1Y2023.DP03?q=dp03
    https://data.census.gov/table/ACSDP1Y2023.DP04?q=dp04
    https://data.census.gov/table/ACSDP1Y2023.DP05?q=dp05

NAICS (Business Revenue by Sector) Census Data
       https://data.census.gov/table/ECNBASIC2017.EC1700BASIC?q=NAICS



## Conclusion

This analysis demonstrates a strong correlation between higher city walkability scores and enhanced urban quality, reflected in both the Built Environment and Socioeconomic indicators. Notably, the top 15 most walkable cities exhibit significantly higher median home values, lower poverty and unemployment rates, reduced car dependency for commuting, and superior access to public transit. Among the factors analyzed, proximity to public transportation emerges as a key lever cities can utilize to improve walkability. Small population CSAs, which lag by almost a full point in walkability score when compared to Medium and Large CSAs - On average they have generally very poor access to public transportation, this presents a clear opportunity: implementing robust public transit options now could significantly boost their walkability before future growth increases implementation challenges. Strategic investment in public transit appears crucial for developing more walkable, equitable, and economically vibrant cities.
