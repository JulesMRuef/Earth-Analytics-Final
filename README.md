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

- **Habitat and Range:** Found in prairies, meadows, and open woodlands, with a native range extending from Canada to Mexico. Today it is generally found from the east coast to the Rocky Mountains, Arizona, Wyoming, and Utah.
  
- **Thermal Range:** Thrives in warm temperatures, with optimal growth between 75 to 90 degrees Fahrenheit. Goes dormant during colder winter months. A native, warm season (C4), perennial with short, scaly rhizomes. It grows from 3 to 8 feet tall, with glabrous culms and flat, 10 to 20 inches long leaves. 

- **Physical Characteristics:** Grows in clumps, reaching heights of 3 to 7 feet, with long, narrow, bluish-green leaves. Produces distinctive bronze-colored flower heads in late summer and fall.

- **Ecological Importance:** Plays a crucial role in preventing soil erosion, providing habitat for wildlife, and contributing to ecosystem health.

- **Cultural Significance:** Historically used by Native American tribes for basket weaving, thatching, and as a food source for wildlife.

- **Adaptation:** Adapted to deep, moist soils ranging from heavy clays to sand with a pH range of 4.8 to 8.0. Has a medium tolerance to salinity and drought.

- **Uses:** Highly palatable to all classes of livestock, suitable for grazing and hay. Provides ground cover and nesting areas for gamebirds and songbirds. Also used by white-tailed deer for cover. Has cultural significance, historically used by Native Americans for basket weaving.

Understanding the dynamics of *Sorghastrum nutans* is essential for monitoring the impacts of environmental changes on native plant species and ecosystems.

![Indian Grass Map](https://soilcropandmore.info/crops/Grasses/Indiangrass/Sorghastrum_nutans_map.jpg)












# Indiangrass Habitat Suitability Model

## Overview

This repository contains a habitat suitability model for *Sorghastrum nutans* (Indiangrass), a native warm-season grass. The model assesses environmental factors to predict suitable habitats for Indiangrass growth.

## Table of Contents

- [Description](#description)
- [Distribution](#distribution)
- [Adaptation](#adaptation)
- [Uses](#uses)
- [Ethnobotany](#ethnobotany)
- [Status](#status)
- [Wetland Indicator](#wetland-indicator)
- [Weedy or Invasive](#weedy-or-invasive)
- [Planting Guidelines](#planting-guidelines)
- [Management](#management)
- [Pests and Potential Problems](#pests-and-potential-problems)
- [Environmental Concerns](#environmental-concerns)
- [Control](#control)
- [Seeds and Plant Production](#seeds-and-plant-production)
- [Cultivars, Improved, and Selected Materials](#cultivars-improved-and-selected-materials)
- [Literature Cited](#literature-cited)
- [Running the Code for Any Grassland](#running-the-code-for-any-grassland)

## Description

Indiangrass (*Sorghastrum nutans*) is a native warm-season perennial grass known for its adaptation to a variety of habitats. This README provides information on its characteristics, distribution, adaptation, uses, and more.

## Distribution

Indiangrass is found from the east coast to the Rocky Mountains, Arizona, Wyoming, and Utah. For current distribution, please consult the Plant Profile page for this species on the PLANTS Web site.

## Adaptation

Indiangrass is adapted to deep, moist soils ranging from heavy clays to sand with a pH range of 4.8 to 8.0. It has a medium tolerance to salinity and drought. Indiangrass is adapted to periodic burning and survives by sprouting from underground rhizomes.

## Uses

- **Forage:** Highly palatable to all classes of livestock, suitable for both grazing and hay when properly managed.
- **Wildlife:** Provides ground cover and nesting areas for gamebirds and songbirds. White-tailed deer utilize the tall grass for cover. Native bees gather nesting materials, and it serves as a larval host and adult food source for certain butterfly species.

## Ethnobotany

The Lakota name for Indiangrass means "red grass with fluffy light–colored end." Native Americans wove Indiangrass into baskets and mats, often dyeing it and decorating it with beads, bark, or quills.

## Status

Not listed as threatened or endangered.

## Wetland Indicator

Indiangrass is a facultative upland plant throughout the continental United States. It usually occurs in non-wetlands but may occur in wetlands.

## Weedy or Invasive

This plant may become weedy or invasive in some regions or habitats and may displace desirable vegetation if not properly managed.

Please consult the PLANTS Web site and your state’s Department of Natural Resources for this plant’s current status.

## Planting Guidelines

Indiangrass seed is planted from mid-winter to late spring depending on planting conditions. The preferred method is using a no-till seed drill equipped with a native grass seed box. Contact your local NRCS Field Office or cooperative extension service for recommended planting dates.

## Management

During the establishment year, use mowing and herbicide applications to control annual grasses and weeds in seedling stands. Mowing should leave 6 to 12 inches of grass stubble. Grazing is not recommended during the establishment year.

Indiangrass is tolerant to fire, but its response may differ in monoculture or mixed stands. Consult local authorities for guidance on prescribed burning.

## Pests and Potential Problems

Indiangrass may serve as a host plant for leaf spot pathogens. Pests include rust fungi. Environmental concerns include potential spread to adjacent areas.

## Environmental Concerns

Control methods include tillage and broad-spectrum herbicides. Consult local agricultural extension specialists for guidance.

## Seeds and Plant Production

Production fields should be fertilized and limed based on soil test recommendations after plants have had at least one growing season to establish.

Indiangrass seed fields reach their peak production at three years and have a productive stand life of 10 to 15 years.

## Cultivars, Improved, and Selected Materials

This section provides information on various cultivars, germplasms, and their areas of origin.

## Literature Cited

A list of references providing further information on Indiangrass.



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

2. Install Dependencies:

bash
Copy code
pip install -r requirements.txt
Run the Workflow Script:

bash
Copy code
python habitat_model_workflow.py

3. View Results:

Explore generated figures and model outputs in the designated output directories.

Contact:
For any questions or assistance, please contact [Juilana Ruef] at [juliana.ruef@colorado.edu]. I appreciate your engagement in this habitat modeling project and look forward to your insights!


**Project by [Juliana Ruef] | [12/14/23]**


