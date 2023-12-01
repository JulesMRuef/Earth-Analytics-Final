# Earth Analytics Final


Our changing climate is changing where key grassland species can live, and grassland management and restoration practices will need to take this into account.



In this project, you will create a habitat suitability model for Sorghastrum nutans, a grass native to North America. In the past 50 years, its range has moved northward. The model will be based on combining multiple data layers related to soil, topography, and climate. You will also demonstrate the coding skills covered in this class by creating a modular, reproducible workflow for the model.

You will create a reproducible scientific workflow
Your workflow should:

Define your study area: Download the USFS National Grassland Units and select your study site(s). Undergraduate students may choose one grassland; graduate students must choose AT LEAST 2.
Fit a model: For each grassland:
Download model variables as raster layers covering your study area envelope, including:
At least one soil variable from the POLARIS dataset
Elevation from the SRTM (available from the APPEEARS API)
At least one climate variable from the MACAv2 dataset, accessible from Climate Toolbox. *Undergraduate students may download a single year and scenario; Graduate students should download at least two)
Calculate at least one derived topographic variable (slope or aspect) to use in your model. You probably will wish to use the xarray-spatial library, which is available in the latest earth-analytics-python environment (but will need to be installed/updated if you are working on your own machine). Note that calculated slope may not be correct if you are using a CRS with units of degrees; you should re-project into a projected coordinate system with units of meters, such as the appropriate UTM Zone.
Harmonize your data - make sure that the grids for each of your layers match up. Check out the ds.rio.reproject_match() method from rioxarray.
Build your model. You can use any model you wish, so long as you explain your choice. However, if you are not sure what to do, we recommend building a fuzzy logic model (see below).
Present your results in at least one figure for each grassland/climate scenario combination.
If you are unsure about which model to use, we recommend using a fuzzy logic model
To train a fuzzy logic habitat suitability model:

Research S. nutans, and find out what optimal values are for each variable you are using (e.g. soil pH, slope, and current climatological annual precipitation).
For each digital number in each raster, assign a value from 0 to 1 for how close that grid square is to the optimum range (1=optimal, 0=incompatible).
Combine your layers by multiplying them together. This will give you a single suitability number for each square.
Optionally, you may apply a threshold to make the most suitable areas pop on your map.


https://github.com/earthlab-education/Earth-Analytics-2023-01-Intro/issues/634#issue-2015535090
