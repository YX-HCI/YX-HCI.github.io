---
layout: page
title: Urban Big Data and Interactive Analytics <a href="https://yx-hci.github.io/assets/pdf/urbanbigdata.pdf" target="_blank" rel="noopener noreferrer" class="float-right"><i class="fas fa-file-pdf"></i></a>
description: Leveraging Urban Big Data for Informed Business Location Decisions.
img: assets/img/project_imgs/UrbanBigData/Urbanbigdata.png
importance: 2
tags: "#Urban Big Data, #Spatial Computing, #Business Strategies. "
category: "VIS"
---

Here’s the project paper: 
- **Xiang, Y.**, Chang, D., Feng, X. (2023). Leveraging Urban Big Data for Informed Business Location Decisions: A Case Study of Starbucks in Tianhe District, Guangzhou City. In *IEEE International Conference on Industrial Engineering and Engineering Management (IEEM)*,IEEE. (Accepted). 



With the development of the information age, cities provide a large amount of data that can be analyzed and utilized to facilitate the decision-making process. Urban big data and analytics are particularly valuable in the analysis of business location decisions, providing insight and supporting informed choices. By examining data relating to commercial locations, it becomes possible to analyze various spatial characteristics and derive the feasibility of different locations. This analytical approach contributes to effective decision-making and the formulation of robust location strategies. To illustrate this, the study focuses on Starbucks cafes in the Tianhe District of Guangzhou City, China. Utilizing data visualization maps, the spatial distribution characteristics and influencing factors of Starbucks locations are analyzed. By examining the geographical coordinates of Starbucks, main distribution characteristics are identified. Through this analysis, it explores the factors influencing the spatial layout of commercial store locations, using Starbucks as a case study. The findings offer valuable insights into the management of industrial layout and the location strategies of commercial businesses in urban environments, opening avenues for further research and development in this field.

# Methodology

At the level of research methodology, we collect data by processing and visualizing them for different aspects of analysis, to derive the influence of different factors.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanBigData/1.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 1. Framework of research methodology..
</div>

## 1)	Data collection
To ensure accuracy, we collected the precise geographical coordinates from latest months and real-time data of the distribution of Starbucks in Tianhe district. The use of a map POI coordinates grabber tool facilitates the collection of latitude and longitude data for the required elements, enabling accurate representation of their positions on the base map. This includes information on the surrounding land use, demographics, competitor locations, and infrastructure availability. Comprehensive dataset provides a more holistic understanding of the factors influencing business location decisions. 
## 2)	Date visualization
We combined with GIS tools to achieve accurate visualization of location data, which enable the creation of interactive maps, heat maps, and 3D visualizations, allowing for a more comprehensive exploration of the relationships between different variables and their impact on business location decisions.
## 3)	Data analysis
Taking Starbucks in Tianhe District as an example, we use big data visualization to analyze location. Due to the huge amount of data collected, we divide the data into three major categories: land price, human flow, and transportation:
### a.Land use &Land price:
According to the nature of different land, select a number of representative target points in Tianhe District and calculate the average land price.
### b.Flow of people:
Using Tencent's pedestrian traffic detection as a tool to record real-time traffic data. The tool collects video based on the embedded camera lens, then performs parallax calculation on the video images of the two cameras to form a 3D image of the person in the video, and then analyzes the shape and height of the human body, sets the statistics by region and direction to calculate the number of passengers.
### c.Transportation:
The traffic information is abstracted into public transportation coverage, including the radiation coverage density of bus stops and subway  stations. The locations of relevant bus stops and subway stations are collected and analyzed for subsequent correlation analysis.

# Result Analysis
## Spatial Distribution Analysis 
### 1)	Spatial distribution status:
According to the official data of Starbucks, there were 175 Starbucks coffee shops in Guangzhou, including 143 central urban areas (Liwan District, Yuexiu District, Haizhu District, Tianhe District, Baiyun District, Huangpu District), accounting for 81.7%, 26 in the suburbs (Panyu District, Huadu District), 6 in the remote suburbs (Nansha District, Zengcheng City, Conghua City), showing a rapid decline from the center. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanBigData/2.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 2.The spatial distribution of Starbucks(left) and some major commercial areas(right) in Guangzhou.
</div>

The concentration of Starbucks stores predominantly centers around the core of Tianhe District, exhibiting a pronounced correlation with the patterns of public traffic flow.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanBigData/3.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 3.The spatial distribution of Starbucks in Tianhe District of Guangzhou.
</div>


The distribution of Starbucks stores in Tianhe District reveals four primary typologies: street-facing storefronts on the first floor of large shopping malls, non-1st floor storefronts within large shopping malls, strip storefronts, and street-facing storefronts on the first floor of commercial office buildings, as well as non-1st floor street storefronts within commercial office buildings. Among these categories, street-facing storefronts on the first floor of large shopping malls account for 40% of the selected sites, occupying prime street-level spaces with high pedestrian footfall. Additionally, favorable locations include prominent business districts, strip commercial districts, and business office areas. It is noteworthy that only two Starbucks establishments are situated within the subterranean dining spaces of office buildings.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanBigData/3.5.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Table 1. The Spatial Distribution Status of Starbucks in Tianhe District.
</div>


### 2)	Main influencing factors analysis

**a. Land Use & Price:**

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanBigData/4.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 4.The spatial distribution of Starbucks in Tianhe District of Guangzhou.
</div>

**b. Transportation:**

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanBigData/5.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 5. The spatial distribution of starbucks with land price of Tianhe District of Guangzhou.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanBigData/6.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 6. The spatial distribution of Starbucks with subway station of Tianhe District of Guangzhou.
</div>

**c. Flow of Pedestrians:**

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/UrbanBigData/7.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 7.The spatial distribution of Starbucks with pedestrians’s flowrate in Tianhe District of Guangzhou
</div>


### 3)	Spatial distribution characteristic:
Based on a comprehensive analysis, the spatial distribution characteristics of Starbucks in the Tianhe District can be delineated by several key observations. Firstly, Starbucks stores are predominantly concentrated in the central area of Tianhe District, with a discernible decrease in density as one moves away from the center. Additionally, Starbucks exhibits a strong presence in prosperous regions, specifically within the business district and areas characterized by higher housing prices. Moreover, a significant correlation is observed between the Starbucks index and the density of bus and subway stations, indicating the influential role of public transportation availability in determining Starbucks locations. Lastly, Starbucks demonstrates a clear preference for densely populated areas, highlighting a strategic emphasis on regions with vibrant human activity and substantial foot traffic. By examining these spatial patterns and understanding the underlying factors, valuable insights can be gained for effective decision-making and the development of robust location strategies.


# Discussion
The spatial distribution characteristics of Starbucks refer to the patterns and arrangement of Starbucks locations in a given geographical area. These characteristics provide insights into how Starbucks chooses its store locations and the factors that influence their distribution. While the specific spatial distribution characteristics may vary depending on the region or city under study, our study yielded some generalized findings.

- **Concentration in urban centers:** Starbucks stores tend to be highly concentrated in urban centers, such as city downtowns or central business districts.   These areas typically attract a large volume of foot traffic and offer a diverse range of commercial and cultural activities.
- **Proximity to transportation hubs:** Starbucks often selects locations near transportation hubs, such as train stations, bus terminals, or major intersections. These areas serve as convenient meeting points and attract commuters, travelers, and individuals passing through the vicinity.Its well-developed transportation infrastructure and high population density establish it as a prominent location for Starbucks' spatial distribution.
- **Presence in high-traffic areas:** Starbucks stores are commonly found in high-traffic areas with a significant number of pedestrians, including busy shopping streets, commercial complexes, and popular tourist destinations. These locations provide increased visibility and accessibility to a larger customer base.
- **Clustered in commercial and retail zones:** Clustered in commercial and retail zones: Starbucks tends to cluster its stores within commercial and retail zones, where there is a concentration of other businesses, shops, and entertainment venues. This clustering strategy allows Starbucks to benefit from the existing customer flow and capitalize on the synergy created by neighboring establishments

Through  analysis, it can be seen that the city's urban centers, transportation hubs, high-traffic areas, and commercial and retail zones of a city are the main factors affecting the location of Starbucks. It is important to acknowledge that these spatial distribution characteristics may vary depending on the specific context and market conditions. Nevertheless, this paper's examination of the spatial distribution of Starbucks in a particular area offers valuable insights into their site selection strategy and the factors that influence their location decisions.
