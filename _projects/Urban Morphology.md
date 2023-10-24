---
layout: page
title: Urban Computing and Human Behavior <a href="https://yx-hci.github.io/assets/pdf/urbanmor.pdf" target="_blank" rel="noopener noreferrer" class="float-right"><i class="fas fa-file-pdf"></i></a>
description: Exploring the Correlation between Urban Microclimate Simulation and Urban Morphology.
img: assets/img/project_imgs/UrbanMorphology/UrbanMorphology.png
importance: 3
tags: "#Urban Morphology, #Modeling and Simulation."
category: "VIS"
---


Here’s the project paper: 
- **Xiang, Y.**, Chang, D., Cheng, J. (2023). Exploring the Correlation between Urban Microclimate Simulation and Urban Morphology: A Case Study in Yeongdeungpo-gu, Seoul. In *IEEE International Conference on Industrial Engineering and Engineering Management (IEEM)*,IEEE. (Accepted). 



In the context of diverse urban morphologies shaped by various social backgrounds and planning policies, this study delves into the intricate relationship between urban morphology, computing techniques, and human behavior insights. The focus is on understanding how urban morphology influences local microclimates, particularly outdoor temperatures, and its implications for addressing the heat island effect. Specifically, our research centers on Yeongdeungpo-gu, Seoul, South Korea, during the summer season, where we examine temperature variations around different types of residential buildings. Employing advanced urban microclimate simulation techniques, we employ a multidimensional approach involving building clusters' morphological indices. Our findings reveal a significant correlation: high-rise residential buildings tend to exhibit noticeably higher outdoor temperatures compared to their low-rise counterparts. Additionally, the presence of open spaces emerges as a critical factor in tempering high neighborhood temperatures. This research underscores the significance of factoring in the interplay among urban morphology, human activity, and managerial decision-making in urban assessments. By bridging the gap between data-driven urban morphology analysis, cutting-edge computing tools, and insights into human behavior, it contributes to informed urban design decisions. 

# Methodology

While numerous studies have explored the impacts of increasing urban building density on urban microclimate, particularly focusing on the significant heat island effect, few have delved into the influence of urban morphology on outdoor temperature, which is also a contributing factor to the urban heat island effect. 

Therefore, our study aims to investigate the relationship between outdoor air temperature, urban microclimate, and various urban forms using ENVI-met, a 3D modeling software that enables high-resolution simulation of outdoor microclimates. This software has become a fundamental tool in urban and building design research. Through this process, we examine a specific residential area in Seoul and analyze how outdoor temperatures differ between two types of residential buildings during the summer. 

This study focuses the outdoor temperature of different residential blocks in Seoul, South Korea, as the research subjects, summarizes the research status and trend of urban microclimate and outdoor temperature related fields, and uses the ENVI-met software as numerical simulation method and application.



<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanMorphology/1.1.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Figure 1. Framework of research and simulation methodology.
</div>


### 1) Selection and Classification Principles for the Research Site
The research site is chosen to encompass a variety of building types, including high-rise and low-rise structures. This selection aims to eliminate interference factors stemming from different land masses, such as varying building densities, traffic conditions, wind speeds, and outdoor temperatures. When classifying building types, plots with well-defined boundaries are preferred. Considering these factors, the Yongdeungpo Area in Seoul is chosen as the research site.

<div class="row justify-content-sm-center justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanMorphology/2.1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanMorphology/2.2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 2. Left: Surrounding condition map.  Right: Satellite map.
</div>

By assessing the overall height of building cluster, using road and the nature building cluster characteristic as as a natural boundary to classify. Two residential building types(a. high-rise building and b. low-rise building)are selected.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanMorphology/3.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Figure 3. Classification standard.
</div>

The streetscape fabric of the two urban residential zones, along with their related spatial pattern indexes, are outlined below.

<div class="row justify-content-sm-center justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanMorphology/4.1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanMorphology/4.2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 4. Left: Road-network.  Right: High-rise and low-rise building.
</div>

### 2)	3D Modeling process

Through meticulous on-site investigations, we obtained precise specifications for the smallest single building in the selected area. Using a 2D road network map as a foundation, we incorporated green plants along the roadside to ensure the model reflected the actual conditions on the ground. The heights of the buildings in the model were determined based on pre-surveyed data, ranging from 15m to 100m. Once the specifications were finalized, we proceeded to model the area with great precision using the Envi-met software, to simulate and analyze the microclimate characteristics of the area in a highly accurate and detailed manner .

<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanMorphology/5.1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanMorphology/5.2.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 5. Left: View of 2D Model.   Right: View of 3D Model.
</div>


### 3)	Data selection and input: 

In ENVI-met, two types of data are required for model calculations. Firstly, the basic data includes time duration and fundamental climate parameters such as temperature, humidity, wind speed, and pressure. We obtained these data from the Korea Meteorological Administration's online public information and inputted them into the software accordingly. Secondly, specific values like relative humidity at 2m or other variables were calculated by referencing the ENVI-met Manual Contents and interpreting the data.

# Result Analysis
### A. Observation of Overall Simulation Results

**1) High-rise Building Block Has Higher Temperature:** By examining the temperature profile at one o'clock in the afternoon (Figure 11), it becomes evident that the high-rise buildings consistently exhibit higher temperatures compared to the low-rise buildings. This temperature difference persists throughout the day.

<div class="row justify-content-sm-center justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanMorphology/6.1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanMorphology/6.2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 6. Simulation result from 11 a.m. to 2 p.m.(left) and  1 p.m.(right).
</div>

**2) Open Space Helps to Relieve High Block Temperatures:** In a specific area with 15m buildings and a lower floor area ratio, a significant proportion of open space is present. The temperature profile demonstrates that this area generally experiences lower temperatures, indicating that the presence of open spaces contributes to temperature relief. These green pockets provide shade, promote evapotranspiration, and reduce the heat island effect, all of which contribute to the cooling of the immediate environment. 

**3)	Air Flow Helps to Lower the Neighborhood Temperature:** The narrow pathway nestled amidst the low-rise buildings consistently maintains significantly lower temperatures compared to its surrounding areas. The mechanism at play here involves the unrestricted flow of air, which carries away excess heat and promotes heat dispersion, which underscores the beneficial impact of enhanced air circulation in lowering local temperatures.

<div class="row justify-content-sm-center justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanMorphology/7.1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanMorphology/7.2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 7. Simulation result from 11 a.m. to 2 p.m.(left) and  1 p.m.(right).
</div>


### B. Analysis and Optimization of Simulation Results

**1) Building Density:** Under the condition of similar building heights, higher building density leads to higher temperatures within the block area. Therefore, when planning building layouts, a balanced consideration of density is crucial to optimize design strategies.


**2) Building Height:** 
Higher building heights correspond to higher air temperatures within the block area. During the observed periods, area 2 experiences higher temperatures than area 1. Therefore, it is important to strike a reasonable balance in building heights and avoid excessive concentration of high-rise buildings to maintain a balanced outdoor temperature.

**3) Air Flow and Wind Tunnel:** 
High-speed air flow can alleviate high temperatures within the region. Fluid mechanics principles demonstrate that objects obstruct fluid flow, reducing the flow rate. Our findings confirm that high-rise buildings impede air flow in the area, resulting in reduced wind speeds. Hence, high-speed air flow proves effective in alleviating regional high temperatures. Additionally, wind tunnels can mitigate local high temperatures. 

The region indicated as area 1 in Figure 15 represents a narrow road within a densely populated low-rise residential block, acting as a wind tunnel. Due to the swift wind speed within the tunnel, heat dissipates more rapidly, resulting in lower air temperatures compared to the surrounding areas. Therefore, urban morphology considerations should include the incorporation of intervals to create temperature-reducing areas, optimizing design strategies.
	
# Discussion
Our research serves as a preliminary investigation into the variations in summer outdoor temperatures and microclimates across diverse residential areas in Yeongdeungpo district. We aim to identify the factors influencing these differences and explore the synergistic effects of various morphological indicators on street spatial texture and microclimate. By conducting simulations and comparative analyses, we aim to offer valuable insights and suggestions to enhance urban climate adaptability through optimized urban spatial morphology in future urbanization developments.

Through our study, we recognize that the design and layout of residential areas play a significant role in shaping the microclimate. The morphological indicators, such as building density, building height, open space, and street layout, collectively impact the local climate. By investigating these factors and their interrelationships, we aim to shed light on the potential strategies and interventions that can be employed to enhance microclimatic conditions. By conducting comprehensive simulations and analyzing the positive microclimate characteristics observed in different residential areas, our research aims to provide practical and actionable recommendations. These suggestions will serve as valuable guidelines for urban planners and developers, helping them optimize urban spatial morphology to improve urban climate adaptability.
