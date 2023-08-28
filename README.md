# SEED_v1.0
Streamflow Extreme Event Dataset (SEED)

# Streamflow Extreme Event Dataset (SEED)
Streamflow Extreme Event Dataset (SEED) is a dataset that includes both flood and drought extreme events for the USGS sites collocated with the NHDPlus stream reaches over the entire contiguous United States (CONUS). SEED includes the extreme flood and drought events during the period 1980-2020.   

The following steps were used to develop SEED for the extreme flood events: 
**Step 1:** Collect streamflow data for the USGS sites that are collocated with the NHDPlus stream reaches 
**Step 2:** Select annual maximum streamflow series for each site over the entire data period
**Step 3:** Fit probability distribution to the annual maximum series 
**Step 4:** Calculate return period for each annual maximum streamflow value in the annual maximum series
**Step 5:** Identify the date of occurrence for each annual maximum streamflow value 
At the end, the tables are created for each USGS site in every state. So the SEED for flood events contains station id, date of occurrence, annual maximum streamflow value, exceedance probabilities, and return periods. 

**SEED table for the extreme flood events:** 

![image](https://github.com/shahab122/SEED/assets/28275758/556dc96d-10fc-431d-9349-6915474f9008)
