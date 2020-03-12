<p align="center"></p>

# STD Cases on the Rise in the US

## Context

The rate of STD infections are on the rise in the US.  This project started as an attempt to determine the cause of the recent rise in infections, however it was best to identify determine who is most at risk so those people could better protect themselves. 

## Table of Contents

- [Context](#Context)
- [Content](#Content)
- [Analysis](#Analysis)
- [Illustrations](#Illustrations)
- [Recommendations](#Recommendations)
- [Data Sources](#Data-Sources)
- [Next steps](#Next-steps)

## Content

The data collected is mostly numeric and compiled from publicly accessible government resources, namely the [Center for Disease Control](https://wonder.cdc.gov/controller/datarequest/D128) (CDC) and the [Bureau of Economic Analysis](https://www.bea.gov/) (BEA).  

Due to the limitations of the CDC web based interface, nine different datasets were collected, each with over 200 rows.  The site offered minimal searching, sorting, and grouping options, causing the segmented data downloads.  There was also a low timeout for the queries, which required data collection in off peak hours.

There were numerous caveats with collecting the data, most notably summarizing all STDs while maintaining granularity with categorical data.  The CDC search tool returned a plain text file that was not spaced properly horizontally and vertically.  Aside from the mechanics of collecting the data, there were several important pieces of data that would have been beneficial.  The most beneficial would be the method of infection.  As people who test positive are tracked, including a simple 

## Analysis

- R-squared = 1 on raw data. 
- Strong multicollinearity indicated by the pair plot.
- P-values indicate only 3 engineered features for the model
- Added external economic data with no affect

## Illustrations 


![Ages](img/infections_age.svg)  
![MF](img/mf_inf_percent.svg)  
![GDP](img/statecasesvsgdp.svg) 

## Recommendations

To lower your risk, select someone who is post college age, choose a state with high GDP (CA, NY, TX), and male! 

## Data-Sources

- [CDC](https://wonder.cdc.gov/controller/datarequest/D128)  
- [BEA](https://www.bea.gov/)

## Next-steps  
 
Moving forward, I'd like to find the infection method to add to the model.  I'd also like to have permission from dating apps to pull their usage numbes (by state.)

