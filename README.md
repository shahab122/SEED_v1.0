# SEED_v1.0
Streamflow Extreme Event Dataset (SEED)

# Streamflow Extreme Event Dataset (SEED)

![image](https://github.com/shahab122/SEED_v1.0/assets/28275758/36f9d9ed-fdb1-4c65-b742-d3f592719277)

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

Now, the following steps were used to develop SEED for the extreme hydrological drought events:  
**Step 1:** Collect streamflow data for the USGS sites that are collocated with the NHDPlus stream reaches
**Step 2:** Calculate the annual total flow for each year during 1980-2020
**Step 3:** Calculate moving average flow for a moving window or duration of 1, 2, 3, 4, 5 years and so on
**Step 4:** Calculate long-term average annual flow or threshold flow
**Step 5:** Calculate % deficit of moving average annual flow relative to the threshold flow for each moving window or duration 
**Step 6:** Identify % deficit series for each USGS site
**Step 7:** Develop cumulative distribution functions or SDF curves for each duration by fitting Weibull’s plotting position formula to the % deficit series

Good news is that the above steps were implemented in the Python based Drought Analysis Tool called pyDAT. The pyDAT tool was used to construct the SDF curves and develop SEED for the drought events. Please note that pyDAT is under development by Savalan Neisary. 

**SEED table for the extreme drought events:**
																
![image](https://github.com/shahab122/SEED/assets/28275758/939e0204-450e-4f75-a60e-5ba9e15221ed)

## Application of SEED

SEED can be used to develop our understanding of “appropriate model formulations” to address diversity of dominant hydrologic processes, select the best model structure and discretization to represent these dominant hydrological processes. Thus, SEED can help researchers of CIROH (as well as outside CIROH) to develop multi-model mosaic in the NextGen framework. So why are we evaluating the model performance? Because we need the appropriate model formulations that perform we in all hydroclimatic conditions over entire CONUS and other parts of North America as well. 

We also developed a Python-based toolfor model evaluation and we call it the Streamflow Evaluator Tool or SET. It is a Python-based, user-friendly, fast, and model agnostic streamflow evaluator tool. This tool can used for any model that uses NHDPlus dataset. It allows a user to evaluate the performance of the National Water Model as well as any other models. This Python-based tool helps visualize the results and investigate the model performance interactively. The current version of the tool is available on github.

https://github.com/whitelightning450/Streamflow_Evaluator

The SET can be used to show the relationship between LULC and the model performance, thus efforts are being made towards connecting regionally specific hydrology to the model performance. 

SEED supports repeatable and quantifiable hydrologic model evaluation, especially when coupled with the Streamflow Evaluator Tool (SET). This workflow helps to better understand dominant hydrological processes as well as when, where, and why they occur and paves a way toward selecting the appropriate model mosaic. Coupled SEED and SET is a framework to develop understanding of performance of different models and configurations that lead towards selecting appropriate models for use in the NextGen framework. SEED can be applied in the event-based evaluation of hydrologic models and can tell us where model performance needs improvement.   

### Data Access

#### How to use SEED Coupled with SET? 

##### NOTE: THIS TOOL IS UNDER DEVELOPMENT
