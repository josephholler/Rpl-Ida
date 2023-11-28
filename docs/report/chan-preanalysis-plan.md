# Pre-analysis Plan for RPl-Ida

## Elise Chan, 11/28/2023

### Analysis

I plan to follow the same procedure as Dr. Holler's original project. However, due to changes to Twitter when it got rebranded as X, I can no longer access Twitter data via API. As a result, I will have to deviate from the original study in the way I normalize the data for mapping. 

To perform my analysis, I plan to take the following steps:

1. Run the original Hurricane Dorian code to gain an understanding of the procedure. 
2. For the Hurricane Ida code, remove all code fetching data from an API. I have the Twitter data for Ida downloaded. However, it is stored in four different queries so I will merge them using the *rbind* function. 
3. Because I no longer have access to Twitter directy, I need to normalize the data over a different value than Twitter baseline data. Instead, I can use Census population for the spatial extent of the Twitter queries. This may may be an overestimate of Twitter users. 

### Results

I will produce the same figures as the original Hurricane Dorian case study. This includes:
- A map of clusters of Twitter activity during Hurricane Ida, as measured by the Normalized Difference Tweet Index developed by Dr. Holler
- A map of tweet locations during Hurricane Ida
- Number of tweets per hour during the duration of Hurricane Ida
- A word network of words used in tweets relating to Hurricane Ida

### Discussion

First, I will discuss the results in the context of Hurricane Ida and its spatial and temporal extent. Then, I will compare the results to those from the Hurricane Dorian study (if I get the code to function without too much extra difficulty) to see how trends compared between the two hurricanes. The Hurricanes differ in spatial extent, but the normalized map will allow me to look at trends in clustering. 
