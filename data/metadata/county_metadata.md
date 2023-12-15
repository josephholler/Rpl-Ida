- `Title`: County Data
- `Abstract`: County data was retrived using a Census API. This data comes from the 2021 ACS 5-year survey. The 5-year survey was selected over the 1-year survey because the 1-year only includes counties with population over 60,000 people.
- `Spatial Coverage`: Counties of the states within the Twitter search radius. FIPS codes of the states inclded: 01, 05, 08, 09, 10, 11, 12, 13, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 31, 33, 34, 35, 36, 37, 38, 39, 40, 42, 44, 45, 46, 47, 48, 50, 51, 54, 55
- `Spatial Resolution`: County
- `Spatial Reference System`: NAD83 (CRS:4269)
- `Temporal Coverage`: 2021
- `Temporal Resolution`: NA
- `Lineage`: The first six variables were retrieved using a Census API, and the code is included in the study report. Tweet variables were derived from a combination of the Census and Twitter data (see Twitter_metadata.md). 
- `Distribution`: Census data is in the public domain.
- `Constraints`: None
- `Data Quality`: Margin of error is reported for population, but many values are missing.
- `Variables`: 

| Label | Alias | Definition | Type | Accuracy | Domain | Missing Data Value(s) | Missing Data Frequency |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| STATEFP | state FIPS code | unique ID for each state | integer | ... | ... | ... | ... |
| COUNTYFP | county FIPS code | unique ID for each county | integer | ... | ... | ... | ... |
| GEOID | geographic ID | unique ID for geometry | integer | ... | ... | ... | ... |
| ALAND | area land | area of county in square meters | numeric | ... | ... | ... | ... |
| POP | population | ... | integer | ... | ... | ... | ... |
| MOE | margin of error | margin of error for population | numeric | ... | ... | NA | frequent |
| DENSITY | population density | calculated by dividing population by area of land (converted to square miles) | numeric | ... | ... | ... | ... |
| event_tweets | ... | number of Hurricane Ida tweets from the county | integer | ... | ... | NA replaced with 0 | ... |
| twitter_pop | twitter population | POP divided by 10,000 to estimate number of generic tweets | numeric | ... | ... | ... | ... |
| tweetrate | tweet rate | event_tweets / twitter_pop | numeric | ... | ... | ... | ... |
| ndti | normalized difference tweet index | normalized difference between event_tweets and twitter_pop, between -1 and 1 | numeric  | ... | ... | NA replaced with 0 | ... |