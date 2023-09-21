---
layout: post
title: Assessing Campaign Performance Using Chi-Square Test For Independence
image: "/posts/ab-testing-title-img.png"
tags: [Tableau, Data Analysis]
---

In this project we apply Chi-Square Test For Independence (a Hypothesis Test) to assess the performance of two types of mailers that were sent out to promote a new service! 

# Table of contents

- [00. Project Overview](#overview-main)
    - [Context](#overview-context)
    - [Actions](#overview-actions)
    - [Results & Discussion](#overview-results)
    - [Data Overview & Preparation](#data-overview)

___

# Project Overview  <a name="overview-main"></a>

### Context <a name="overview-context"></a>

As part of this project, we were contacted by the DSI organization to analyze earthquakes over a one month period in 2022. This client is looking to expand operations and is looking for areas to consider expansion into.  Building costs and maintenance can be higher in those areas where earthquakes are prevalent. Our client asked for us to provide the following analysis:geographical analysis containing the location of the earthquake, the ten largest earthquakes by location, the percentage of earthquakes that occurred based on the broad location of the earthquake, frequency by location, average magnitude by location, and maximum magnitude by location.  


<br>
<br>
### Actions <a name="overview-actions"></a>

For this deliverable, we provided a Tableau dashboard with visuals reprensenting the key requirements.
Those requirements were:

* Provide geograhical analysis of all earthquakes 
* Provide analysis on the top 10 largest earthquakes
* Provide analysis on the percentage of earthquakes based on the broad location identified
* Provide analysis for the frequency based on location
* Provide analysis for the average magnitutde based on location
* Provide analysis for the maximum magnitude based on location

### Results & Discussion <a name="overview-results"></a>

Based on our observations, we can provide the following insights for frequency of earthquakes based on broad geographical location:

* North America(Highest): **58%** rate of earthquakes
* Central America(Lowest): **3%** rate of earthquakes

We can provide the following insights for maximum magnitude of earthquakes based on geographical location:

* Vanuatu(Highest): **88** magnitude based on 2 events
* Michigan(Lowest): **8** magnitude based on 1 event

We can provide the following insights for the 10 largest earthquakes based on geographical location:

* Vanuatu experienced the top 2 largest earthquakes based on 2 events during this time period
* Tonga experienced the 3rd and 4th largest earthquakes based on 4 evens

<br>
<br>
# Data Overview & Preparation  <a name="data-overview"></a>

The client provided us with the necessary file and miminal manipulation was needed.  There was some data cleansing that was required which included clean up of inconsisent formatting of column values.
<br>
<br>
