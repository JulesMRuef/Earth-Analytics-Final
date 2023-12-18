# Habitat Suitability Modeling for Sorghastrum nutans (S. Nutans)

[![DOI](https://zenodo.org/badge/687226006.svg)](https://zenodo.org/doi/10.5281/zenodo.8408496)


<div style="text-align:center">
    <img src="https://cdn.plantatlas.org/img/specimens/USF/32833.jpg" alt="Image 1" width="325"/>
    <img src="https://objects.liquidweb.services/images/201409/richard_orr_14913356819_04b763fd74_z.jpg" alt="Image 2" width="325"/>
</div>

- **Image 1:**
  [Description of Image 1]

- **Image 2:**
  [Description of Image 2]

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

*Sorghastrum nutans*, commonly known as Indiangrass, is a warm-season grass native to North America.

## Habitat and Range

Found in prairies, meadows, and open woodlands, with a native range extending from Canada to Mexico. Today it is generally found from the east coast to the Rocky Mountains, Arizona, Wyoming, and Utah.

## Thermal Range

Thrives in warm temperatures, with optimal growth between 75 to 90 degrees Fahrenheit. Goes dormant during colder winter months. A native, warm season (C4), perennial with short, scaly rhizomes.

## Physical Characteristics

Grows in clumps, reaching heights of 3 to 7 feet, with long, narrow, bluish-green leaves. Produces distinctive bronze-colored flower heads in late summer and fall.

## Uses

- **Forage:** Highly palatable to all classes of livestock, suitable for both grazing and hay when properly managed.
- **Wildlife:** Provides ground cover and nesting areas for gamebirds and songbirds.

## Ecological Importance

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

Anderson, J., & Morse, S. (2012). Topographical Location Has Little Effect on Andropogon gerardii and Sorghastrum nutans. Tillers, 4, 1-3.https://digital-grinnell.nyc3.cdn.digitaloceanspaces.com/ojs-static/tillers/article/view/29/29

Plant database. Lady Bird Johnson Wildflower Center - The University of Texas at Austin. (n.d.). https://www.wildflower.org/plants/result.php?id_plant=sonu2

Silletti, A., & Knapp, A. (2002). Long-term responses of the grassland co-dominants Andropogon gerardii and Sorghastrum nutans to changes in climate and management. Plant Ecology, 163, 15-22.https://link.springer.com/article/10.1023/A:1020320214750

Sorghastrum Nutans. Sorghastrum nutans (Indiangrass, Yellow Indiangrass) | North Carolina Extension Gardener Plant Toolbox. (n.d.). https://plants.ces.ncsu.edu/plants/sorghastrum-nutans/

## Project Workflow - a Reproducible Scientific Workflow:

### 1. Define Study Area
- Download the USFS National Grassland Units shapefile.
- Select study site(s) within the grasslands.

### 2. Download Model Variables
- Utilize the APPEEARS API for at least one soil variable from the POLARIS dataset.
- Obtain elevation data from SRTM via the APPEEARS API.
- Access MACAv2 dataset
- Calculate a derived topographic variable (e.g., slope or aspect) using xarray-spatial.

### 3. Harmonize Data
- Ensure grid alignment for all layers using the `ds.rio.reproject_match()` method from rioxarray.

### 4. Build the Model
- Build a fuzzy logic model
- Assign values (0 to 1) for each variable based on optimal values for S. nutans.
- Combine layers by multiplication to get a single suitability score for each grid square.

### 5. Present Results
- Generate figures for each grassland/climate scenario using the fuzzy logic model.
- Evaluate and visualize habitat suitability for Sorghastrum nutans.





## Contact:
For any questions or assistance, please contact [Juilana Ruef] at [juliana.ruef@colorado.edu]. I appreciate your engagement in this habitat modeling project and look forward to your insights!


**Project by [Juliana Ruef] | [12/14/23]**


