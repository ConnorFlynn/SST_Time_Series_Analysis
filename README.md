# SST_Time_Series_Analysis

This exploratory analysis for Statics for Environmental Data Science (EDS 223) examines Sea Surface Temperature data from the [NOAA Coral Reef Watch CoralTemp dataset](https://coastwatch.pfeg.noaa.gov/erddap/griddap/NOAA_DHW.html). CoralTemp is a global sea surface temperature data product used primarily for coral bleaching monitoring. The dataset contains several data products based on 5 geostationary and 3 polar-orbiting satellites. The spatial resolution of the data is 5km with complete daily spatial coverage of the ocean from 1985-04-01 to present.

The 5km grid for this analysis encompasses Honolii, Hawaii. This marine ecosystem off the Hilo coast of the Big Island is known to house to coral that is showing resilliency toward warming sea surface temperatures caused by climate change. According to NOAA, corals experience stress if water reaches 1°C warmer than the highest expected annual temperature (Glynn and D'Croz, 1990). Thus, the bleaching threshold is defined as 1°C warmer than the maximum monthly mean temperature. 
Coral can be heat tolerant for a variety of reasons. This analysis explores the hypothesis that the coral of Honolii reef have the ability to adapt to heat by hosting a symbiont algae that increases their bleaching threshold by approximately 1.5 degree celsius compared to non heat tolerant coral.

While Sea Surface Temperature, especially from a 5 km resolution, is only of the many things that influence marine ecosystem health, it can be extremely useful in understanding and managing marine ecosystems. This analysis:
1. Imports over 35 years of daily sea surface temperature data from CoralTemp for Honolii, Hawaii.
2. Estimates the linear relationship between time and mean sea surface temperature, using 'lm()' to fit a regression model using Ordinary Least Squares (OLS).
3. Runs a classical decomposition model to examone seasonality and overall trend in mean monthly sea surface temperature over time.
4. Uses two different models to foreast sea surface temperature:
    1. Allows us to predict future coral bleaching events for both heat tolerant and non heat tolerant coral based on their different bleaching thresholds. 
