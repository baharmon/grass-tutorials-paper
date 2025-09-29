---
title: 'Tutorials for the GRASS geocomputation engine'
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

This collection of tutorials is an introduction to the GRASS geospatial processing engine. GRASS is an open source computational engine for spatiotemporal data management, analysis, modeling, and simulation [@GRASS]. As an engine that can be integrated in data science pipelines with shell scripting, Python, R, Jupyter, and Colab, there are many ways to use GRASS.  While GRASS already had extensive documentation, tutorials were needed to introduce the many ways to interface with GRASS. These open education tutorials - which cover integrations, core features, and disciplinary applications - were developed as part of an effort to grow the GRASS community. The tutorials were built with Quarto and deployed as webpages paired with Jupyter computational notebooks. The tutorials are available at https://grass-tutorials.osgeo.org under both the GNU Free Documentation License v1.2 or later and the Creative Commons Attribution-ShareAlike 4.0 International License.

# Statement of Need

*Include a Statement of Need section, explaining how the submitted artifacts contribute to computationally enabled teaching and learning, and describing how they might be adopted by others.*

* Growing the GRASS ecosystem
  * GRASS has extensive documentation, but lacked official tutorials
    * Manual pages, api documentation, programming manual, etc.
    * Community developed tutorials
      * Not maintained by GRASS Dev Team
  * Current GRASS roadmap calls for new tutorials
    * Encourage community growth
    * Demonstrate integration  into data science pipelines
  * Introduction to GRASS as geospatial engine
    * Examples of how to interface with engine needed
      * GUI, CLI, Py, R, Cloud, Jupyter, etc.
  * Implementation based on teaching experiences
    * HTML: NCSU Geospatial Modeling (GIS/MEAS 582) [@Petras:2015]
    * HTML: NCSU UAS Mapping and Analysis (GIS/MEAS 584)
    * Jupyter: NCSU Geospatial Computing and Simulation (GIS714) [@Haedrich:2023]

<!-- The current roadmap for GRASS calls for new tutorials on introductory and advanced topics to encourage community growth and new tutorials to demonstrate how the engine can be integrated into data science pipelines.  -->

# Description

<!-- Describe the learning objectives, content, instructional design, and experience of use in teaching and learning situations. -->

## Learning Objectives

These tutorials were developed to teach the fundamentals of geoprocessing with GRASS, integrations of GRASS into data science pipelines, and disciplinary applications of GRASS. The tutorials were designed for self-study by learners of all levels, integration into courses, and deployment in workshops.

## Instructional Design

The tutorials were designed to teach a computational approach to thinking about spatiotemporal phenomena through different interfaces to the GRASS engine. Drawing on the education benefits of computational notebooks [@Barba:2022], the tutorials were designed as modules for reuse and remixing, as worked examples to reduce cognitive load, as interactive lessons for active learning and engagement, as scaffolded prose and code to structure learning, and as computable content to teach computational thinking. The tutorials introduce geocomputational concepts through worked examples that synthesize prose explanations, graphics, and runnable code. The tutorials, which range from introductory to advanced, have a modular design for reuse and remixing so that learners can choose their own course of study and teachers can select modules for their lesson plans. The tutorials build in complexity from introductory to core to disciplinary modules. A set of getting started tutorials introduce different ways to interface with the GRASS engine. The core tutorials cover important concepts such as geovisualization, map algebra, geospatial modeling, and the temporal framework. Disciplinary tutorials demonstrate applications for GRASS in domains such as climatology, ecology, hydrology, geomorphology. The disciplinary tutorials build engagement by working through applications in the learner’s domain and thus motivate further exploration. Throughout the tutorials, different ways to interface with GRASS are presented as tabs in code blocks, so that learners can work their way through the same tutorial repeatedly using increasingly challenging interfaces – building proficiency first with the graphical user interface (GUI), then with the command line interface (CLI), and finally with the Python application programming interface (API).

## Implementation

This collection of tutorials was published using Quarto as web documents paired with computational notebooks. To reach a broad audience, the tutorials are published as web documents for immediate, easy access via web browsers. When appropriate, the web documents are accompanied by computational notebooks for the sake of interactivity, engagement, and geocomputational thinking. The tutorials – which are built and deployed using the Quarto scientific publishing system (Quarto) – are written in Markdown with YAML frontmatter. Tutorials are composed in Markdown for human-readable source code, efficient version control, executable code blocks for different interfaces, rendering in multiple formats, and reproducibility. As this open education project aims to teach different ways to interface with GRASS, executable code for multiple relevant interfaces such as the GUI, CLI, Python, or R can be included in tutorials as tabsets. Once tutorials have been written, they are reviewed by the GRASS Development Team, rendered as web documents and Jupyter notebooks, and deployed to an Open Source Geospatial Foundation website. The source code for the tutorials is built in the GitHub repository https://github.com/OSGeo/grass-tutorials and deployed to the website https://grass-tutorials.osgeo.org using GitHub Actions. 

## Contents / Tutorials

This official collection of tutorials is maintained by the GRASS Development Team as part of the documentation for the GRASS geocomputational engine (\autoref{table:core}). This ensures that tutorials undergo rigorous review, tutorials are maintained and updated as GRASS evolves, and issues are promptly addressed. The website also includes a curated collection of community contributed tutorials that are hosted on external websites and maintained by their creators (\autoref{table:community}). 

: Official GRASS tutorials \label{table:core}

| Modules     | Tutorials                                              | Level        | Language            |
|-------------|--------------------------------------------------------|--------------|---------------------|
| Get Started | Get started with GRASS GUI                             | Beginner     | English             |
|             | Get started with GRASS & Python in Jupyter Notebooks   | Beginner     | English             |
|             | Get started with GRASS in Google Colab                 | Beginner     | English             |
|             | Get started with GRASS in Jupyter Notebooks on Windows | Beginner     | English             |
|             | Get started with GRASS & R: the rgrass package         | Advanced     | English             |
| General     | Basics of map algebra                                  | Beginner     | English             |
|             | Making plots with GRASS                                | Beginner     | English             |
|             | Visualizing and modeling terrain from DEMs in GRASS    | Beginner     | English, Portuguese |
|             | Modeling Movement in GRASS                             | Advanced     | English, Portuguese |
|             | Introduction to remote sensing with GRASS              | Beginner     | English             |
|             | Procedural noise                                       | Intermediate | English             |
|             | Quick comparison: R and Python GRASS interfaces        | Intermediate | English             |
| Time series | Introduction to time series in GRASS                   | Intermediate | English             |
|             | Temporal subset, import and export                     | Intermediate | English             |
|             | Temporal aggregations                                  | Advanced     | English             |
|             | Temporal algebra                                       | Advanced     | English             |
|             | Temporal accumulation                                  | Advanced     | English             |
|             | Temporal gap-filling                                   | Advanced     | English             |
|             | Temporal query with vector data                        | Advanced     | English             |
| Earthworks  | Basic earthworks                                       | Beginner     | English             |
|             | Gully modeling                                         | Beginner     | English             |
|             | Coastal infrastructure                                 | Beginner     | English             |
|             | Terrain synthesis                                      | Intermediate | English             |

: Community contributed tutorials \label{table:community}
| Modules | Tutorials | No. | Level    | Language |
|---------|-----------|-----|----------|----------|
| ...     | ...       | ... | ...      | ...      |

## Story

*Tell us the story of the project: how did it come to be?*

Please add to the story!

* Teaching experiences
  * HTML: NCSU Geospatial Modeling (MEAS582/GISXXX) [@Petras:2015]
  * NCSU Geospatial Modeling (GIS/MEAS 582) [White 2023 - 2025]
  * NCSU UAS Mapping and Analysis (GIS/MEAS 584) [White 2024-2025]
  * Jupyter: NCSU Geospatial Computing and Simulation (GIS714) [@Haedrich:2023]

## Acknowledgements

The initial development of these tutorials was partially supported by the U.S. National Science Foundation under Grant [2303651](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2303651).

## References
