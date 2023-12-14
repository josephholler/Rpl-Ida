- `Title`: Tweets about Hurricane Ida
- `Abstract`: Tweets containing key words about Hurricane Ida were searched using the Twitter API. 
- `Spatial Coverage`: 1000 miles radius around coordinates 36, -87. 
- `Spatial Resolution`: Coordinates attached to tweets refer to a city, neighborhood, or a specific point of interest. 
- `Spatial Reference System`: NAD83 (CRS:4269)
- `Temporal Coverage`: Notes in the code say tweets were searched on September 2-10, 2021, however the dates of the actual tweets rane from August 29-September 10, 2021.
- `Temporal Resolution`: Tweet times are recorded down to the second.
- `Lineage`: This data was retrieved using a Twitter API, and the code is included in the study report. However, the code no longer works due to restrictions on Twitter APIs. 
- `Distribution`: Twitter data is not allowed to be shared on GitHub. Thus, tweets are stored in a private folder ignored by GitHub.
- `Constraints`: Twitter data may not be posted on GitHub.
- `Data Quality`:
- `Variables`: The raw twitter data has 90 variables. Those relevant to this study are included below.

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
