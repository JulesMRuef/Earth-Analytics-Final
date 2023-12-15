# Habitat Suitability Modeling for Sorghastrum nutans

<div style="text-align:center">
    <img src="https://sowwildnatives.com/images/thumbs/0000951_indian-grass-sorghastrum-nutans.jpeg" alt="Image 1" width="325"/>
    <img src="https://cdn.plantatlas.org/img/specimens/USF/32833.jpg" alt="Image 2" width="325"/>
    <img src="https://objects.liquidweb.services/images/201409/richard_orr_14913356819_04b763fd74_z.jpg" alt="Image 3" width="325"/>
</div>

- **Image 1:**
  [Description of Image 1]

- **Image 2:**
  [Description of Image 2]

- **Image 3:**
  [Description of Image 3]

# Habitat Suitability Modeling for *Sorghastrum nutans*

## Introduction

Our changing climate is affecting the distribution of key grassland species, necessitating a reevaluation of grassland management and restoration practices. In this project, we aim to create a habitat suitability model for *Sorghastrum nutans* (Indiangrass), a native North American grass that has exhibited a northward range expansion in the past 50 years.

This repository contains a habitat suitability model for *Sorghastrum nutans*. The model integrates multiple data layers related to soil, topography, and climate to understand and predict suitable habitats for *S. nutans*.

## Table of Contents

1. [About *Sorghastrum Nutans*](#about-sorghastrum-nutans)
2. [Habitat and Range](#habitat-and-range)
3. [Thermal Range](#thermal-range)
4. [Physical Characteristics](#physical-characteristics)
5. [Uses](#uses)
6. [Ecological Importance](#ecological-importance)
7. [Ethnobotany](#ethnobotany)
8. [Weedy or Invasive](#weedy-or-invasive)
9. [Pests and Potential Problems](#pests-and-potential-problems)
10. [Control](#control)
11. [Literature Cited](#literature-cited)
12. [Running the Code for Any Grassland](#running-the-code-for-any-grassland)

## About *Sorghastrum nutans*

*Sorghastrum nutans*, commonly known as Indiangrass, is a warm-season grass native to North America. Key characteristics include:

### Habitat and Range

Found in prairies, meadows, and open woodlands, with a native range extending from Canada to Mexico. Today it is generally found from the east coast to the Rocky Mountains, Arizona, Wyoming, and Utah.

### Thermal Range

Thrives in warm temperatures, with optimal growth between 75 to 90 degrees Fahrenheit. Goes dormant during colder winter months. A native, warm season (C4), perennial with short, scaly rhizomes.

### Physical Characteristics

Grows in clumps, reaching heights of 3 to 7 feet, with long, narrow, bluish-green leaves. Produces distinctive bronze-colored flower heads in late summer and fall.

### Uses

- **Forage:** Highly palatable to all classes of livestock, suitable for both grazing and hay when properly managed.
- **Wildlife:** Provides ground cover and nesting areas for gamebirds and songbirds.

### Ecological Importance

Plays a crucial role in preventing soil erosion, providing habitat for wildlife, and contributing to ecosystem health.

- **Cultural Significance:** Historically used by Native American tribes for basket weaving, thatching, and as a food source for wildlife.

## Adaptation

Indiangrass is adapted to deep, moist soils ranging from heavy clays to sand with a pH range of 4.8 to 8.0. It has a medium tolerance to salinity and drought. Indiangrass is adapted to periodic burning and survives by sprouting from underground rhizomes.

## Ethnobotany

The Lakota name for Indiangrass means "red grass with fluffy light–colored end." Native Americans wove Indiangrass into baskets and mats, often dyeing it and decorating it with beads, bark, or quills.

## Weedy or Invasive

This plant may become weedy or invasive in some regions or habitats and may displace desirable vegetation if not properly managed.

Please consult the PLANTS Web site and your state’s Department of Natural Resources for this plant’s current status.

## Pests and Potential Problems

Indiangrass may serve as a host plant for leaf spot pathogens. Pests include rust fungi. Environmental concerns include potential spread to adjacent areas.

## Literature Cited

A list of references providing further information on Indiangrass.

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

![Indian Grass Map](https://soilcropandmore.info/crops/Grasses/Indiangrass/Sorghastrum_nutans_map.jpg)

## Project Workflow

### 1. Define Study Area
- Download the USFS National Grassland Units shapefile.
- Select study site(s) within the grasslands. Undergraduates choose one; graduates choose at least two.

### 2. Download Model Variables
- Utilize the APPEEARS API for at least one soil variable from the POLARIS dataset.
- Obtain elevation data from SRTM via the APPEEARS API.
- Access MACAv2 dataset through Climate Toolbox for at least one climate variable. Undergraduates download for a single year and scenario; graduates download at least two.
- Calculate at least one derived topographic variable (e.g., slope or aspect) using xarray-spatial.

### 3. Harmonize Data
- Ensure grid alignment for all layers using the `ds.rio.reproject_match()` method from rioxarray.

### 4. Build the Model
- Choose a model; we recommend a fuzzy logic model.
- Assign values (0 to 1) for each variable based on optimal values for S. nutans.
- Combine layers by multiplication to get a single suitability score for each grid square.
- Optionally, apply a threshold for visualization.

### 5. Present Results
- Generate figures for each grassland/climate scenario using the fuzzy logic model.
- Evaluate and visualize habitat suitability for Sorghastrum nutans.

## Running the Code

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/your-repository.git
   cd your-repository












Contact:
For any questions or assistance, please contact [Juilana Ruef] at [juliana.ruef@colorado.edu]. I appreciate your engagement in this habitat modeling project and look forward to your insights!


**Project by [Juliana Ruef] | [12/14/23]**


