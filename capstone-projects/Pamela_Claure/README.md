# Understanding Precipitation Partitioning and Hydrologic Impacts in Mountainous Catchments
This repository contains data and scripts necessary for reproducing the Mill Creek catchment model.

## Summary
In the mountainous western United States, snowmelt is the primary source of downstream water supply, but a warming climate threatens the timing and quantity of future water resources. 
As precipitation shifts from snow to rain, the hydrologic impacts on streamflow and groundwater recharge remain poorly understood. 
This project aims to investigate how precipitation partitioning affects hydrological processes in mountainous catchments under changing climate conditions. 
Specifically, it will assess the impact of this shift on streamflow timing and quantity, as well as groundwater recharge, using ATS modeling for integrated hydrology and land surface interactions. 
The study will focus on the Mill Creek watershed within the Jordan River basin, leveraging historical climate and hydrologic data from USGS and NOAA, 
and testing hypothetical climate scenarios to predict future precipitation patterns. 
Expected outcomes include an improved understanding of how changing precipitation affects hydrologic partitioning, 
contributing to predictive models for the Great Salt Lake basin and supporting sustainable water management strategies for stakeholders in the region.

## Methods
- This is the aplication of the Amanzi-ATS model with the Watershed Workflow

- The study area is the Mill Creek catchment in the Jordan River from the Great Salt Lake basin


## Repository Structure
```
|-- data
|-- model
|   |-- inputs
|   `-- outputs
|-- scripts
`-- results
|   |-- figures
```
- `data`: provides data needed to run the model (includes the main inputs to run the watershed workflow)
- `model`: provides input files  for the Amanzi-ATS model. The input daymet data is stored in forlders Scenario 1 (partition threshold 0 °C), Scenario 2 (partition threshold +2 °C) and Scenario 3 (partition threshold -2°C).
			To run the model please change include the files in the Sneraio folder into the processed folder.
			Aditionally in the output folder a comparison of the water balance for the three scenarios is incorporated.
- `scripts - results`: provides the jupyter notebooks for pre - processing model files to prepare the input for ATS and the post processing includes the results analysys and the graphs generated as part of the analysis. 
