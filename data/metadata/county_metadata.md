- `Title`: County Data
- `Abstract`: County data was retrived using a Census API. This data comes from the 2021 ACS 5-year survey. The 5-year survey was selected over the 1-year survey because the 1-year only includes counties with population over 60,000 people.
- `Spatial Coverage`: Counties of the states within the Twitter search radius. FIPS codes of the states inclded: 01, 05, 08, 09, 10, 11, 12, 13, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 31, 33, 34, 35, 36, 37, 38, 39, 40, 42, 44, 45, 46, 47, 48, 50, 51, 54, 55
- `Spatial Resolution`: County
- `Spatial Reference System`: NAD83 (CRS:4269)
- `Temporal Coverage`: 2021
- `Temporal Resolution`: NA
- `Lineage`: This data was retrieved using a Census API, and the code is included in the study report. 
- `Distribution`: Census data is in the public domain.
- `Constraints`: None
- `Data Quality`: Margin of error is reported for population, but many values are missing.
- `Variables`: 

| Label | Alias | Definition | Type | Accuracy | Domain | Missing Data Value(s) | Missing Data Frequency |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| status_id | tweet ID | unique ID assigned to every tweet| integer | ... | ... | ... | ... |
| created_at | time created | ... | yyy-mm-dd hh:mm:ss | ... | ... | ... | ... |
| text | tweet content | ... | character string | ... | ... | ... | ... |
| place_type | geographic subregion | city, neighborhood, poi | character string | ... | ... | ... | ... |
| geo_coords | geographic coordinates |lat, long | list of numbers | ... | ... | NA | frequent |
| coords_coords | reversed coordinates |long, lat (R reads as x, y) | list of numbers | ... | ... | NA | frequent |
| bbox_coords | bounding box coordinates | 4 long and 4 lat coordinates marking the edges of the region for place type | list of numbers | ... | ... | NA | ... |
| lat | latitude | latitude coordinates from coords_coords or centroid of place_type bounding box | number | ... | ... | ... | ... |
| lng | longitude | longitude coordinates from coords_coords or centroid of place_type bounding box | number | ... | ... | ... | ... |
