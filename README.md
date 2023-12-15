# Habitat Suitability Modeling for Sorghastrum nutans

## Introduction

Our changing climate is affecting the distribution of key grassland species, necessitating a reevaluation of grassland management and restoration practices. In this project, we aim to create a habitat suitability model for *Sorghastrum nutans* (Indiangrass), a native North American grass that has exhibited a northward range expansion in the past 50 years. The model will integrate multiple data layers related to soil, topography, and climate to understand and predict suitable habitats for *S. nutans*.

## Project Goals

1. **Reproducible Scientific Workflow:**
   - Define the study area by downloading the USFS National Grassland Units.
   - Fit a habitat suitability model for *Sorghastrum nutans* in selected grassland areas.
   - Download and preprocess model variables, including soil data from the POLARIS dataset, elevation from the SRTM dataset, and climate data from the MACAv2 dataset.
   - Calculate derived topographic variables, such as slope or aspect, using xarray-spatial.
   - Harmonize data to ensure grid compatibility using the `ds.rio.reproject_match()` method from rioxarray.
   - Build a habitat suitability model, allowing flexibility in the choice of the model (*fuzzy logic model* is recommended for those seeking guidance).

2. **Presentation of Results:**
   - Present results through at least one figure for each grassland/climate scenario combination.
   - If unsure about the model choice, a *fuzzy logic model* is recommended for habitat suitability.
   - Evaluate and interpret the results, considering optimal values for variables such as soil pH, slope, and climatological annual precipitation.

3. **Documentation and Evaluation:**
   - Develop a modular and reproducible workflow for the model, showcasing coding skills covered in the class.
   - Provide clear documentation for each step of the workflow.
   - Use a README file to introduce the project, its objectives, and the methodology employed.

## About *Sorghastrum nutans*

*Sorghastrum nutans*, commonly known as Indiangrass, is a warm-season grass native to North America. Key characteristics include:

- **Habitat and Range:** Found in prairies, meadows, and open woodlands, with a native range extending from Canada to Mexico.
  
- **Thermal Range:** Thrives in warm temperatures, with optimal growth between 75 to 90 degrees Fahrenheit. Goes dormant during colder winter months.

- **Physical Characteristics:** Grows in clumps, reaching heights of 3 to 7 feet, with long, narrow, bluish-green leaves. Produces distinctive bronze-colored flower heads in late summer and fall.

- **Ecological Importance:** Plays a crucial role in preventing soil erosion, providing habitat for wildlife, and contributing to ecosystem health.

- **Cultural Significance:** Historically used by Native American tribes for basket weaving, thatching, and as a food source for wildlife.

Understanding the dynamics of *Sorghastrum nutans* is essential for monitoring the impacts of environmental changes on native plant species and ecosystems.

**Project by [Juliana Ruef] | [12/14/23]**


