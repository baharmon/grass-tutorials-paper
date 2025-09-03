---
title: 'GRASS Tutorials'
tags:
  - GRASS
authors:
  - name: Brendan A. Harmon
    orcid: 0000-0002-6218-9318
    affiliation: 1
  - name: Veronica Andreo
    orcid: 0000-0002-4633-2161
    affiliation: 2
  - name: Anna Petrasova
    orcid: 0000-0002-5120-5538
    affiliation: 3
  - name: Vaclav Petras
    orcid: 0000-0001-5566-9236
    affiliation: 3
  - name: Caitlin Haedrich
    orcid: 0000-0003-4373-5691
    affiliation: 3
  - name: Corey White
    orcid: 0000-0002-2903-9924
    affiliation: 3
  - name: Laura Belica
    orcid: 0000-0001-9684-087X
    affiliation: 3
affiliations:
 - name: Louisiana State University, United States
   index: 1
   ror: 05ect4e57
 - name: Instituto Gulich, Argentina
   index: 2
   ror: 00pw52a85
 - name: North Carolina State University, United States
   index: 3
   ror: 04tj63d06
date: 2 September 2025
bibliography: paper.bib

---

<!-- ![Figure \label{fig:figure_1}](figure_1.png){ width=100% } -->

# Summary

`Describe the submission and explain its eligibility for JOSE.`

* Overview of GRASS
  * GRASS as geoprocessing engine [@GRASS]
    * Features [@Gebbert:2017; @Haedrich:2023]
    * Integrations
    * Well documented, but lacking official tutorials
* GRASS Tutorials
  * Tutorials with computational notebooks
    * Integrations
    * Core features
    * Thematic topics
  * Dual licensed GFDL-1.2-or-later & CC-BY-SA-4.0
  * Audience: GRASS and wider FOSS4G community

# Statement of need

`Include a Statement of Need section, explaining how the submitted artifacts contribute to computationally enabled teaching and learning, and describing how they might be adopted by others.`

* Growing the GRASS ecosystem
  * GRASS has extensive documentation, but lacked official tutorials
    * Manual pages, api documentation, programming manual, etc.
    * Community developed tutorials
      * Not maintained by GRASS Dev Team
  * Introduction to GRASS as geospatial engine
    * Examples of how to interface with engine needed
      * GUI, CLI, Py, R, Cloud, Jupyter, etc.


# Description / Features

`Describe the learning objectives, content, instructional design, and experience of use in teaching and learning situations.`

## Learning Objectives

* Learn the fundamentals of geoprocessing with GRASS
* Learn disciplinary applications of GRASS

## Instructional Design

* Design
  * Learning modules for self-study, classes, & workshops
  * Modular design for reuse and remixing
  * Scaffolded: getting started > core features > disciplinary topics
  * Interactivity for active learning
  * Worked examples for reduced cognitive load
  * Computational thinking with live coding
  * Scaffolding of explanations and code
* Audience
  * GRASS community of practice
    * Academics, professionals, & agencies
    * OSGeo Foundation
    * Broader FOSS4G community
  * Beginners to advanced
  * Self-learners: getting started tutorial series
* Mode
  * Online tutorials with computational notebooks
* Implementation, Infrastructure, & Deployment
  * Quarto > GitHub Pages
    * HTML pages & Jupyter notebooks

## Contents / Tutorials

* Tutorials
  * Get started
    * Get started with GRASS GUI
    * Get started with GRASS & Python in Jupyter Notebooks
    * Get started with GRASS & R: the rgrass package
    * Get started with GRASS in Google Colab
    * Get started with GRASS in Jupyter Notebooks on Windows
  * Core features
    * Basics of map algebra
    * Making plots with GRASS
    * Visualizing and Modeling Terrain from DEMs in GRASS (English & Portuguese)
    * Modeling Movement in GRASS (English & Portuguese)
    * Introduction to remote sensing with GRASS
    * Procedural noise
    * Quick comparison: R and Python GRASS interfaces
  * Disciplinary topics
    * Deep dive into time series analysis with GRASS
      * Introduction to Time Series in GRASS
      * Temporal aggregations
      * Temporal algebra
      * Temporal accumulation
      * Temporal gap-filling
      * Temporal query with vector data
      * Temporal subset, import and export
    * Earthworks
      * Basic earthworks
      * Gully modeling
      * Coastal infrastructure
      * Terrain synthesis

* External Tutorials
  * Physically-based hydrologic modeling using GRASS GIS r.topmodel
  * GRASS for Remote Sensing data processing with Jupyter Notebooks
  * Teledetección, OBIA y series de tiempo
  * GISMentors - GRASS GIS školení
  * GISMentors - Courses
  * Unleash the power of GRASS GIS
  * Deforestation study using GRASS GIS
  * NCSU Geospatial Modeling and Analysis Course
  * Urban growth modeling with FUTURES
  * GIS for Designers
  * Geoprocessamento com GRASS GIS
  * OpenGeoHub 2019: GRASS GIS for environmental monitoring and disease ecology applications
  * Processing lidar and UAV point clouds
  * Tutoriales de GRASS GIS en grasswiki
  * Spatio-temporal data handling and visualization
  * Ecodiv.earth tutorials
    * Species distribution modeling using Maxent in GRASS
    * Mapping the distribution of the White-tailed deer in Minnesota
    * From suitability to suitable regions
    * Tree species diversity distribution

# Story

`Tell us the story of the project: how did it come to be?`

Please add to the story!

* Teaching experiences
  * HTML: NCSU Geospatial Modeling (MEAS582/GISXXX) [@Petras:2015]
  * Jupyter: NCSU Geospatial Computing and Simulation (GIS714) [@Haedrich:2023]

# Acknowledgements

The initial development of these tutorial was partially supported by the U.S. National Science Foundation under Grant [2303651](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2303651).

# References