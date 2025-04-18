# Factors-Influencing-Walkability-A-Comparative-Analysis-Across-US-Combined-Statistical-Areas
Executive Summary
This project investigates the factors influencing walkability across Community Statistical Areas (CSAs) in the United States. Utilizing the EPA's National Walkability Index merged with U.S. Census Bureau data (American Community Survey DP02, DP03, DP04, DP05, and NAICS data), the study explores the correlations between walkability scores and various demographic, socioeconomic, built environment, and commuting characteristics at the CSA level. Key analyses include identifying significant predictors of higher walkability, examining the relationship between commuting behaviors and walkability potential, comparing socioeconomic profiles of high-walkability small CSAs versus low-walkability large CSAs, and exploring potential links between walkability and business activity indicators. The findings aim to provide actionable insights for urban planners, policymakers, and community developers seeking to enhance walkability and its associated benefits (e.g., public health, economic activity, environmental sustainability).

Motivation
My personal experience in Nashville, where pedestrian infrastructure and opportunities feel limited in comparison with highly walkable cities highlight the significant variation in walkability across different landscapes in the US. This observation sparks a critical question: what distinguishes highly walkable places from those that are less accommodating to pedestrians? This project is motivated by the desire to move beyond anecdotal assessments and systematically identify the demographic, socioeconomic, and built-environment characteristics correlated with high walkability using national datasets (EPA NWI, Census ACS). By identifying and understanding the attributes of the most walker-friendly CSAs, this research aims to provide valuable benchmarks and insights for urban planners, policymakers, and communities seeking to enhance pedestrian accessibility and reap the associated benefits in their own areas.	
Data Question(s)
1.)	Which specific demographic factors, socioeconomic factors, and built environment indicators show the strongest correlations with higher National Walkability Index scores?
2.)	How strongly do commuting behaviors relate to walkability scores across different CSAs? Does high walkability correlate with higher non-car commuting?
3.)	When comparing the top 5 highest-walkability small CSAs against the bottom 5 lowest-walkability large CSAs, do the high-walkability small CSAs demonstrate better socioeconomic, and built environment profiles?

Minimum Viable Product (MVP)
1.) A Merged and Cleaned Dataset: A final dataset integrating variables from the EPA National Walkability Index, Census ACS DP02, DP03, DP04, DP05, and NAICS codes, aggregated or matched at the CSA level. 
2.)  Correlation Analysis Results: Statistical summaries quantifying the relationships identified in Data Question 1 (Walkability vs. Demographics, Socioeconomics, Built Environment). 
3.)  Commuting Behavior Analysis: Results addressing Data Question 2 regarding the link between commuting patterns and walkability scores. 
4.)  Comparative CSA Analysis: Results addressing Data Question 3, comparing the socioeconomic profiles of the selected top small and bottom large CSAs based on walkability. 
5.)  Business Correlation Insights: Initial findings or visualizations exploring the relationship outlined in Data Question 4. 
6.)  Key Visualizations: A set of maps, scatter plots, bar charts, or other relevant graphics illustrating the primary findings. 
7.)  Final Report/Presentation: A PowerPoint/PowerBI presentation summarizing the project's motivation, methodology, data sources, key findings for each research question, limitations, and conclusions/recommendations.

Known Issues and Challenges
1.)	Data Granularity: Analyzing data at the CSA level is useful for regional insights but masks significant variations within CSAs. Findings reflect CSA averages and may not apply uniformly to all neighborhoods within a CSA. This was due to the data not being available for CBSA level (more granular) for all CBSAs analyzed.
2.)	Data Integration Complexity: Merging datasets from different sources (EPA, multiple Census tables) with potentially varying geographic identifiers or reference periods required careful cleaning, & alignment. 
3.)	Correlation vs. Causation: The analysis primarily focuses on correlations. While strong correlations suggest relationships, they do not definitively prove causation (ex: does higher income cause higher walkability, or do walkable areas attract higher-income residents, or is it a different factor(s) entirely?).
4.)	NWI Index Limitations: The National Walkability Index is a composite score based on specific built environment factors (ex: intersection density, proximity to transit). It may not capture all aspects relevant to pedestrian experience.

Data Sources
Walkability Index from EPA
https://www.epa.gov/smartgrowth/smart-location-mapping#walkability
DP(Data Profile) DP02-DP05 Census Data
    https://data.census.gov/table/ACSDP5Y2022.DP02
    https://data.census.gov/table/ACSDP1Y2023.DP03?q=dp03
    https://data.census.gov/table/ACSDP1Y2023.DP04?q=dp04
    https://data.census.gov/table/ACSDP1Y2023.DP05?q=dp05
    NAICS (Business Revenue by Sector) Census Data
       https://data.census.gov/table/ECNBASIC2017.EC1700BASIC?q=NAICS

