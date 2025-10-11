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

# Summary

This collection of tutorials is an introduction to the GRASS geospatial processing engine. GRASS is an open source computational engine for spatiotemporal data management, analysis, modeling, and simulation [@GRASS; @Neteler:2008]. As an engine that can be integrated in data science pipelines with shell scripting, Python, R, Jupyter, and Colab, there are many ways to use GRASS.  While GRASS already had extensive documentation of individual processing tools, tutorials were needed to introduce the many ways to interface with the tools and combine them into computational workflows (\autoref{fig:figure_1}). These open education tutorials - which cover integrations, core features, and disciplinary applications - were developed as part of an effort to grow the GRASS community. The tutorials are built with Quarto and are deployed as webpages paired with Jupyter computational notebooks. The tutorials are available at https://grass-tutorials.osgeo.org under both the GNU Free Documentation License v1.2 or later and the Creative Commons Attribution-ShareAlike 4.0 International License.

![Tutorial on using GRASS, NumPy, and Landlab for Scientific Modeling. This tutorial demonstrates a seamless workflow for scientific modeling in Python, showing how gridded data can be passed as arrays between GRASS, NumPy [@Harris:2020], and Landlab [@Barnhart:2020]. \label{fig:figure_1}](figure_1.png){ width=100% }

# Statement of Need

As GRASS has grown from its roots as a desktop geographic information system [@Westervelt:2004], it has evolved into a geocomputational engine with many interfaces. As an engine, it can be integrated in geospatial data science pipelines using shell scripting, application programming interfaces, tangible interfaces [@Petrasova:2018], computational notebooks [@Haedrich:2023], cloud computing environments [@Neteler:2019; @White:2023], or high performance computing environments. While GRASS is well documented with a user manual, developer manuals, and a wiki, it lacked official tutorials. Over the years, the community developed many tutorials across different platforms, but as these are independently maintained, many have become outdated and obsolete. The current roadmap for GRASS – established in 2024 – calls for official new tutorials to encourage community growth and demonstrate integrations in data science pipelines. 

The design and implementation of the new official tutorials for GRASS was based on experience teaching university courses and conference workshops using open educational resources. Over the last decade, the GRASS community has developed many open educational resources, experimenting with delivery via web documents, computational notebooks, and cloud computing services. Online tutorials for GRASS have been built from source in HTML [@Petras:2015], built from Markdown rendered with Hugo, included Jupyter notebooks [@Haedrich:2023], and used cloud computing services such as Google Colab. @Petras:2015 used a modular structure with tabsets to teach the core interfaces for GRASS – the GUI, CLI, and Python API – separating explanatory text introducing geospatial concepts from software specific text for each interface. This scaffolding helps learners to focus on concepts, while building their skills with increasingly complex interfaces. @Haedrich:2023 developed a GRASS–Jupyter integration to incorporate more scripting into a graduate-level course on Geospatial Computing and Simulation. The package extends the existing GRASS Python APIs with data visualization and management tools for the Jupyter environment. The new course materials include Jupyter Notebooks that combine tutorials and assignments, allowing students to write and modify code, interact with examples, and explain their reasoning in markdown, all within a single document. Based on these experiences, our design principles for the new tutorials include teaching geospatial concepts discretely from software specifics to encourage spatial thinking, supporting live coding to encourage computational thinking, and using an open source publishing system to build documents from plain text tracked with version control.

# Description

## Learning Objectives

This collection of tutorials was designed to teach geocomputational thinking using the GRASS geoprocessing engine. To introduce computational approaches [@NRC:2010; @Weintrop:2016] to thinking about space and time, the tutorials cover the fundamentals of geoprocessing with GRASS, integrations of GRASS into data science pipelines, and disciplinary applications of GRASS. The tutorials were designed for self-study by learners of all levels, integration into courses, and deployment in workshops.

## Instructional Design

In order to teach a computational approach to thinking about spatiotemporal phenomena through different interfaces to the GRASS engine, the tutorials were designed: 

* as modules for reuse and remixing, 
* as worked examples to reduce cognitive load, 
* as interactive lessons for active learning and engagement, 
* as scaffolded prose and code to structure learning, 
* and as computable content to teach computational thinking. 

Drawing on the education benefits of computational notebooks [@Barba:2022], the tutorials introduce geocomputational concepts through worked examples that synthesize prose explanations, graphics, and executable code. The tutorials, which range from introductory to advanced, have a modular design for reuse and remixing so that learners can choose their own course of study and teachers can select modules for their lesson plans. The tutorials build in complexity from introductory to core to disciplinary modules. A set of "Getting Started" tutorials introduce different ways to interface with the GRASS engine. The core tutorials cover important concepts such as geovisualization, map algebra, geospatial modeling, and the temporal framework. Disciplinary tutorials demonstrate applications for GRASS in domains such as climatology, ecology, hydrology, geomorphology. The disciplinary tutorials build engagement by working through applications in the learner’s domain and thus motivate further exploration. Throughout the tutorials, different ways to interface with GRASS are presented as tabs in code blocks, so that learners can work their way through the same tutorial repeatedly using increasingly challenging interfaces – building proficiency first with the graphical user interface (GUI), then with the command line interface (CLI), and finally with the Python application programming interface (API).

## Implementation

This collection of tutorials was published using Quarto as web documents paired with computational notebooks. To reach a broad audience, the tutorials are published as web documents for immediate, easy access via web browsers. When appropriate, web documents are accompanied by a downloadable computational notebook, encouraging  interactivity, engagement, and geocomputational thinking. The tutorials – which are built and deployed using the Quarto scientific publishing system [@Quarto] – are written in Markdown with YAML frontmatter. Tutorials are composed in Markdown for human-readable source code, efficient version control, executable code blocks for different interfaces, rendering in multiple formats, and reproducibility. As this open education project aims to teach different ways to interface with GRASS, executable code for multiple relevant interfaces such as the GUI, CLI, Python, or R can be included in tutorials as tabsets. Once tutorials have been written, they are reviewed by the GRASS Development Team, rendered as web documents and Jupyter notebooks, and deployed to an Open Source Geospatial Foundation website. The source code for the tutorials is built in the GitHub repository https://github.com/OSGeo/grass-tutorials and deployed to the website https://grass-tutorials.osgeo.org using GitHub Actions. 

## Content

This official collection of tutorials is maintained by the GRASS Development Team as part of the documentation for the GRASS geocomputational engine (\autoref{table:core}). This ensures that tutorials undergo rigorous review, tutorials are maintained and updated as GRASS evolves, and issues are promptly addressed. The website also includes a curated collection of community contributed tutorials that are hosted on external websites and maintained by their creators (\autoref{table:community}). 

: Official GRASS tutorials \label{table:core}

| Modules      | Tutorials                                               | Level        | Lang.   |
|--------------|---------------------------------------------------------|--------------|---------|
| Integrations | Get started with GRASS GUI                              | Beginner     | En      |
|              | Get started with GRASS & Python in Jupyter Notebooks    | Beginner     | En      |
|              | Get started with GRASS in Google Colab                  | Beginner     | En      |
|              | Get started with GRASS in Jupyter Notebooks on Windows  | Beginner     | En      |
|              | Get started with GRASS & R: the rgrass package          | Advanced     | En      |
| Core         | Basics of map algebra                                   | Beginner     | En      |
|              | Making plots with GRASS                                 | Beginner     | En      |
|              | Visualizing and modeling terrain from DEMs in GRASS     | Beginner     | En & Pt |
|              | Introduction to remote sensing with GRASS               | Beginner     | En      |
|              | Quick comparison: R and Python GRASS interfaces         | Intermediate | En      |
|              | Introduction to time series in GRASS                    | Intermediate | En      |
|              | Temporal subset, import and export                      | Intermediate | En      |
|              | Temporal aggregations                                   | Advanced     | En      |
|              | Temporal algebra                                        | Advanced     | En      |
|              | Temporal accumulation                                   | Advanced     | En      |
|              | Temporal gap-filling                                    | Advanced     | En      |
|              | Temporal query with vector data                         | Advanced     | En      |
|              | Modeling movement in GRASS                              | Advanced     | En & Pt |
| Disciplinary | Basic earthworks                                        | Beginner     | En      |
|              | Gully modeling                                          | Beginner     | En      |
|              | Coastal infrastructure                                  | Beginner     | En      |
|              | Terrain synthesis                                       | Intermediate | En      |
|              | Procedural noise                                        | Intermediate | En      |
|              | Hydro-flattening a digital elevation model              | Intermediate | En      |
|              | Using GRASS, NumPy, and Landlab for scientific modeling | Intermediate | En      |
|              | Estimating wind fetch                                   | Advanced     | En      |
|              | Parallelization of overland flow simulation             | Advanced     | En      |

: Community contributed tutorials \label{table:community}

| Modules      | Tutorials                                                       | No. | Level                   | Lang.   |
|--------------|-----------------------------------------------------------------|-----|-------------------------|---------|
| Integrations | Unleash the power of GRASS GIS                                  | 5   | Beginner - Advanced     | En      |
|              | GRASS for remote sensing data processing with Jupyter Notebooks | 1   | Advanced                | En      |
| Core         | NCSU geospatial modeling and analysis course                    | 13  | Beginner - Intermediate | En      |
|              | Geoprocessamento com GRASS GIS                                  | 1   | Beginner - Intermediate | Pt      |
|              | Tutoriales de GRASS GIS en grasswiki                            | 4   | Beginner - Intermediate | Es      |
|              | GISMentors                                                      | 30  | Beginner - Advanced     | En & Cs |
| Disciplinary | Deforestation study using GRASS GIS                             | 1   | Beginner                | En      |
|              | Teledetección, OBIA y series de tiempo                          | 5   | Beginner - Intermediate | Es      |
|              | GIS for designers                                               | 12  | Beginner - Intermediate | En      |
|              | GRASS GIS for environmental monitoring and disease ecology      | 2   | Beginner - Intermediate | En      |
|              | Processing lidar and UAV point clouds                           | 1   | Beginner - Intermediate | En      |
|              | Physically-based hydrologic modeling using r.topmodel           | 1   | Intermediate            | En      |
|              | Spatio-temporal data handling and visualization                 | 1   | Intermediate            | En      |
|              | Ecodiv.earth tutorials                                          | 16  | Beginner - Advanced     | En      |
|              | Urban growth modeling with FUTURES                              | 1   | Advanced                | En      |

## Acknowledgements

The initial development of these tutorials was partially supported by the U.S. National Science Foundation under Grant [2303651](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2303651).

## References
