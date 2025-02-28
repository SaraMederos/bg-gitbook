---
description: What is BrainGlobe?
---

# About

### Introduction

The core goal of **BrainGlobe** is to develop a suite of Python-based software tools for computational neuroanatomy. We developed several software packages to access, analyze and visualize anatomical data, by ensuring the interoperability of all of **BrainGlobe**'s software we aim to facilitate the development of analysis pipelines and facilitate the process of going from raw data to publication-ready content. By producing a set of high-quality open-access Python packages we aim to accelerate the development of sophisticated analysis tools in python.&#x20;



#### Accessing data

Recent developments in high resolution 3D electronic atlases for many model species and of high-throughput experimental techniques enabled the production of a wealth of anatomical data and the creation of vast open datasets like those from the Allen Institute. Accessing, downloading and using these data remains a challenging task which requires significant programming skills.&#x20;

We aim to facilitate the process of accessing data from available dataset, and for that reason we developed [**morphapi**](morphapi/morphapi.md) **** which can be used to download neuronal morphological data. [**brainrender**](brainrender/untitled.md) **** also provides functionality to download gene expression and mesoscale connectomics data for the mouse brain from the Allen institute.&#x20;

A core step towards facilitating the usage of atlas data was taken by developing **BrainGlobe**'s **AtlasAPI**, the [**AtlasAPI**](bg-atlasapi/introduction.md) **** provides a simple and unified interface for downloading and using atlas data from a number of available atlases, and new atlases can easily be added to the API. This addresses one of the main obstacles when developing software for neuroanatomy: few of the available atlases provide programmatic access to their data, and the APIs used to access the data vary across atlases. This obstacle resulted in most of the available software being dedicated to individual atlases or even datasets, requiring that additional and often duplicated effort be spent in adapting existing software to new atlases. By providing a unified API the AtlasAPI aims to facilitate the development of software capable of working across atlases. The AtlasAPI is used by BrainGlobe software tools like [**cellfinder**](cellfinder/cellfinder-introduction.md) and **brainrender** ensuring that they can be effortlessly adapted to work across atlases.

####

#### Analyzing data

The registration of anatomical data to a reference image (from an atlas) is a crucial step in the analysis of anatomical data. Registering the data enables the comparison of data across individuals and experimental modalities and facilitates the dissemination of anatomical data. It is also indispensable to easily compare user-generated data with data from publicly available datasets.

Registering 3D image data to a reference atlas is a technically demanding task. For this reason we developed [**brainreg**](brainreg/introduction.md), a python-based software tool for the registration of anatomical data

**cellfinder** is a **BrainGlobe** software which uses a deep learning algorithm to identify the location of labelled cells (e.g. expressing a fluorescent protein) across an entire brain. It thus provides a fast,  reliable and reproducable approach to the quantification of data from tracing experiments.&#x20;

####

#### Visualizing data

In addition to downloading and analyzing data, visualization is a crucial step in any analysis pipeline. The creation of images and videos from data is crucial for both inspecting the results of analysis steps and for communicating one's findings. BrainGlobe developed **brainrender** to facilitate the creation of high quality 3D interactive renderings of anatomical data. The necessity to visually explore increasing large and rich datasets requires the creating of 3D interactive renderings: given the complicated 3D structures of many types of data (e.g. neuronal morphologies), 2D alternatives are a poor substitute for 3D renderings. However, the creation of high quality renderings remains a challenging problem. **brainrender** provides a user-friendly interface and a powerful and flexible rendering tool to ensure that any scientist can create rich and beautiful renderings of their anatomical data.



