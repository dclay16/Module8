### Using ERA5 & SPC severe thunderstorm data to investigate the relationship between SSTs and thunderstorm activity in the Plains and Southeast U.S.
**Motivation:** With increasing global air temperatures, as well as SSTs, I want to find out if the increasing SST temperatures are resulting in more, the same, or less thunderstorm activity across the Plains and Southeast states.

**Scientific question to be answered:** Does an increase in SST in the eastern Pacific correlate to an increase thunderstorm activity across the Plains and/or Southeast? Is there more (less) thunderstorm activity during ENSO or other climate phases?

**Datasets to be used:** ERA-5 and SPC Severe Thunderstorm Report Data

European Centre For Medium-Range Weather Forecasts. (2019). ERA5 Reanalysis (Monthly Mean 0.25 Degree Latitude-Longitude Grid) [dataset]. UCAR/NCAR - Research Data Archive. https://doi.org/10.5065/P8GT-0R61

National Weather Service Storm Prediction Center. (2024). Severe Weather Database [dataset]. Severe Thunderstorm Wind Reports. https://www.spc.noaa.gov/wcm/data/1955-2022_wind.csv.zip

National Weather Service Storm Prediction Center. (2024). Severe Weather Database [dataset]. Severe Thunderstorm Hail Reports. https://www.spc.noaa.gov/wcm/data/1955-2022_hail.csv.zip

**Methods:** Used deseasonalized, detrended, and standardized SST, dewpoint, and CAPE data to determine any correlation with SST anomalies using EOF and Pearson Correlations. Further, SPC severe thunderstorm report data across the Plains (region 1) and the Southeast (region 2) will be used with a randon forest regression model to attempt to predict thunderstorm activity, while anlyzing feature importance and multipass permutations within the data.

**Results:** The results of the ERA5 analysis were inconclusive on any significant correlation between SST anomalies and surface dewpoint temperature or CAPE. There were areas across the Gulf of Mexico and the southwestern U.S., as well as the upper Great Lakes and New England regions where there was a stronger correlation. However, the Plains and Southeast dis not display any strong correlation. Using the SPC severe storm report data, there was not a strong relationship between SST and severe thunderstorm reports. The analysis indicated that NAO was a strong feature for both regions in high severe thunderstorm activity, however, the months of April through July apeared to show the greatest influcence on thunderstorm activity.

**Conclusions:** The ERA5 did not show any strong relationship between SST anomalies and dewpoint or CAPE. This was expected due to other factors being invloved in thunderstorm development. These could not be modeled in this project. There is a GLM dataset from GOES-16 that has lightning data from 2018 to the present. This would be a great case for using the data in a shorter time period, as it would validate thunderstorm activity much better than ERA5 or the SPC storm reports. The SPC severe thunderstorm report data was somewhat inconclusive in determing thunderstorm activity. The analysis did indicate that a NAO situation typically produces more severe thunderstorms in both the Plains and Southeast. However, the SPC data only refers to severe thunderstorms that produced damaege that was reported. There are a significant number of thunderstorms that are not severe or do not produce any damage that cannot be account for in this data. The addition of lightning data could increase the accuracy of the outcome of the analysis. 
