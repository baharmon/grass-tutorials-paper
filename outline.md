# Summary

*Describe the submission, and explain its eligibility for JOSE.* 

* Overview of GRASS
  * GRASS as geocomputation engine [@GRASS]
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

*Include a Statement of Need section, explaining how the submitted artifacts contribute to computationally enabled teaching and learning, and describing how they might be adopted by others.*

* Growing the GRASS ecosystem
  * GRASS has extensive documentation, but lacked official tutorials
    * Manual pages, api documentation, programming manual, etc.
    * Community developed tutorials
      * Not maintained by GRASS Dev Team
  * Introduction to GRASS as geospatial engine
    * Examples of how to interface with engine needed
      * GUI, CLI, Py, R, Cloud, Jupyter, etc.


# Description / Features

*Describe the learning objectives, content, instructional design, and experience of use in teaching and learning situations.*

## Learning Objectives

* Learn the fundamentals of geoprocessing with GRASS
* Learn how to integrate GRASS into data science pipelines
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
    * Deep dive into time series analysis with GRASS
      * Introduction to Time Series in GRASS
      * Temporal aggregations
      * Temporal algebra
      * Temporal accumulation
      * Temporal gap-filling
      * Temporal query with vector data
      * Temporal subset, import and export
  * Disciplinary topics
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
  * OpenPlains Tutorials

# Story

*Tell us the story of the project: how did it come to be?*

Please add to the story!

* Teaching experiences
  * HTML: NCSU Geospatial Modeling (MEAS582/GISXXX) [@Petras:2015]
  * Jupyter: NCSU Geospatial Computing and Simulation (GIS714) [@Haedrich:2023]
  * NCSU Geospatial Modeling (GIS/MEAS 582) [White 2023 - 2025]
  * NCSU UAS Mapping and Analysis (GIS/MEAS 584) [White 2024-2025]

# Acknowledgements

The initial development of these tutorial was partially supported by the U.S. National Science Foundation under Grant [2303651](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2303651).

# References