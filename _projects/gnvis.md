---
layout: page
title: Generative Design & Visualization <a href="https://yx-hci.github.io/assets/pdf/gnvis.pdf" target="_blank" rel="noopener noreferrer" class="float-right"><i class="fas fa-file-pdf"></i></a>
description: A Style Matching Approach for the Generative Design of Animated Posters.
img: assets/img/project_imgs/gnvis/gnvis/0.png
tags: "#Generative Design, #Visualization, #Style-matching, #Visual Analytics. "
importance: 1
category: "VIS"
---

**Project Video**: 

[//]: # (<video width="320" height="240" controls>)

[//]: # (  <source src="assets/img/video_gnvis.mp4" type="video/mp4">)

[//]: # (</video>)

[//]: # ()


<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="assets/img/vis_v1.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="assets/img/video_gnvis.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>

# Abstract
Animated posters have emerged as a dynamic form of visual expression in the new media era. With their vibrant visuals, engaging narratives, and flexible nature, they offer distinct advantages in enhancing audience experiences and conveying messages effectively. However, existing tools struggle to meet the diverse design needs and high demand. This paper aims to address these gaps by exploring a parametric design method for creating high-quality animated advertising materials more easily. Firstly, a combination of Kansei Engineering and machine learning methods is used to explore the relationship between animation properties and style perception, in order to help designers choose appropriate animations for their posters. Secondly, heuristic rules for poster design are synthesized, leading to the proposal of a parameterized design model. Finally, based on this model and the analysis of user research, a generation tool of animated advertising posters is designed and developed, catering to small and medium-sized businesses as well as junior designers. Users can leverage this platform by providing static materials and customizing styles to obtain visually expressive and communicatively efficient animated posters. In the comparative experiment evaluating poster quality, the results demonstrate that the animated advertising posters produced by the proposed model exhibit significantly greater design diversity and quality compared to existing platforms. Furthermore, a usability test reveals that the generation tool achieves better usability and effectiveness. These findings highlight the potential of the proposed tool to contribute to a more efficient and effective generation process.

# Style Matching Methodology
To quantify the association between explicit animated visual performance and implicit style **semantic features**, essential for achieving a specific animated poster design, we establish an **animated style-matching model**. This model, grounded in the theory of **perceptual engineering**, relies on the construction of an animated style label system and an animated element structure. This framework facilitates a **two-way matching of style and animated effects**, providing a foundation for subsequent **computer-aided generation design**.

## Semantic Keywords Identification
This study uses a funnel model to extract the key semantic features of animated style through three steps: extensive collection of semantic vocabulary, clustering and screening of semantic vocabulary, and validation of the evaluation system to build an animated style labeling system applicable to animated posters.

## Data Acquisition and Cleaning
To create a semantic vocabulary for describing animated advertising poster styles, 446 English words were collected, forming a preliminary corpus. The words underwent cleaning, including translation, de-duplication, and screening. Three design experts with 3 to 5 years of experience conducted preliminary screening, resulting in a final semantic lexicon of 98 adjectives.

## Keywords Clustering and Filtering
To determine classification accuracy, we conducted an open-ended card-sorting experiment with 15 participants having 3-7 years of design experience. Each participant grouped 98 words based on lexical similarity, providing short sentences describing the basis of their grouping, without any limits on the number of groups.

The experimental data were subjected to multidimensional scale analysis to derive Stress and RSQ indices in different spatial dimensions. A lower Stress index indicates a better model fit, while an RSQ value close to 1 signifies better fit quality (preferably >0.6). The analysis determined six dimensions, yielding six-dimensional spatial coordinates. 

These coordinates were then clustered using the K-means algorithm, with the Calinski-Harabasz index (CH index) used for evaluation. Optimal clustering occurred at K=10, with the highest CH index, indicating the best clustering effect and similar-sized clusters. Ultimately, the K-means algorithm clustered the 98 perceptual words into 10 classes based on the six-dimensional spatial coordinates from the multidimensional scale analysis.



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/gnvis/gnvis/1.jpg" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    
</div>





To capture the multi-sense nature of the vocabulary, positive and negative bipolar adjectives were chosen as evaluation dimensions using the semantic differential method. Building on the thesaurus clustering results, we conducted lexical pairing. Utilizing the central words from the 10 class clusters obtained through K-means clustering, representative words were selected for semantic pairing based on the animated dimension of each class description. This process yielded 9 semantic word pairs, serving as evaluation dimensions for the animated style (refer to Table 1).

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/gnvis/gnvis/2.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">

</div>


## Semantic Optimization and Validation
We utilized the semantic difference method to gather users' perceptual cognitive data, analyzed and processed the data using mathematical and statistical methods, such as factor analysis and item analysis.

Then collected 14 classic animated effects, reproduced in GIF format, as experimental stimuli. Combined nine semantic style dimensions with a 7-point Likert scale for animated style evaluation and obtained 30 valid user data, including 10 males and 20 females, with half having no design background.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/gnvis/gnvis/3.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Sample motion effects
</div>



We verified the validity and representativeness of semantic word pairs through experimental recall analysis. Used the critical ratio in item analysis and Pearson correlation for dimension contribution and correlation. Sumed and ranked 420 data sets (30 subjects rating 14 samples), creating high and low groupings, and conducted independent sample t-tests on the two groups with a significance level of 0.01.

After experimental validation, we identified the five most representative semantic word pairs: "direct-moderate," "lively-calm," "popular-futuristic," "smooth-rhythmic," and "exaggerated-restrained" for describing various aspects of animated style.



## Animation Effect Analysis
Four basic units for further research on the semantics of animated style were finally determined based on the structure of animated elements: motion effect, motion duration, amplitude, and speed.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/gnvis/gnvis/4.jpg" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Sample animation effect
</div>


# Joint Matching Approach Based on Back Propagation Neural Network and Genetic Algorithm

After **Dataset Collection and Processing** & **Algorithm Modeling and Fitting**, we constructed a neural network model to investigate the relationship between animated parameters and animated styles.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/gnvis/gnvis/5.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Model structure of BPNN.
</div>



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/gnvis/gnvis/6.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Training and validation loss curves
</div>


In order to achieve this goal quickly and effectively in practical application scenarios, a genetic algorithm is introduced in this study. We integrated the genetic algorithm with BP neural network based on its excellent global search ability, and use the BP network as the fitness function of the genetic algorithm to obtain the animated combination that meets the user’s style intention in a more efficient way. 


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/gnvis/gnvis/7.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Genetic algorithm framework of style-matching model.
</div>


# The Generative Design Platform
## Generative Method

We designed the framework of the platform based on the generation path of animated advertising posters. During the poster design process, the designer sequentially takes four steps: obtaining materials, understanding the content, generating and adjusting parameters, and decoding and displaying.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/gnvis/gnvis/8.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Generation process of animated posters Generation process of animated posters.
</div>



## Design Platform Development
### System Functional Architecture

For the core requirements of in the user operation flow distilled in the previous interview, the corresponding functional solutions are set. The main patterns include design-based generation, and product diagram-based generation. Based on typical usage scenarios and technical implementation considerations, the web application is chosen as the vehicle for the generation tool.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/gnvis/gnvis/9.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Interaction process of the design system.
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/gnvis/gnvis/10.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Design preview page.
</div>

### Prototype Construction
During the prototype phase, a high-fidelity version of the poster generation tool web app was developed using Figma to refine conceptual ideas. The functional prototype, built on the H5 web framework, validated and implemented core functions, specifically the generation process of two models. The prototype comprised web front-end and server back-end components. The front-end, powered by JavaScript's JQuery, facilitated user interactions, file uploads, and data processing. The back-end, written in Python, accepted commands for animated style-matching, scheme parameter generation, and template data access from the front-end.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/gnvis/gnvis/11.png" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     System structure of the prototype.
</div>

# Testing and Evaluation
The matching model between animated attributes and style semantics is obtained through the construction of the preamble, the narrative and design techniques applicable to advertising posters, and a parametric generation model for animated advertising posters is proposed on this basis. We evaluated the effectiveness of this generative model through experiments.

## Poster Generation Effect Test Evaluation


### Evaluation Criteria
The diversity of the generated animated posters was one of the evaluation criteria. This evaluation criteria were thus determined to include the three dimensions of i) poster quality, ii) advertising effectiveness, and iii) generation diversity.


### Analysis of Experimental Results

A total of 24 subjects aged 20-30 years old participated in the memory test and subjective assessment experiment.

1. **Memory test**: the recall of the advertisement is the percent of people who correctly recalled the main product in the poster, and the recall of each poster in the experimental group and the control group was calculated.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/gnvis/gnvis/12.jpg" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Paired t-test for memory test.
</div>



2. **Subjective assessment**: The reliability test on questionnaire scale data yielded a Cronbach alpha coefficient of 0.835, indicating high reliability for subsequent analysis. Posters' quality was evaluated using a user engagement scale, with an overall engagement score calculated from three dimensions. The 12 experimental group posters were scored in three groups, summed for the total score, and compared via paired t-test with a control group.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/gnvis/gnvis/13.jpg" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Quality assessment paired t-test of experimental group-control group
</div>




3. **Generating diversity assessment**: the data analysis method for generating diversity of results is the same as the quality assessment. 


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/gnvis/gnvis/14.jpg" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Diversity assessment paired t-test of experimental group-control group.
</div>

Experimental findings indicate that the proposed animated poster generation model, incorporating style-semantic matching and narrative planning, produces animated advertising posters with enhanced perception, greater marketing impact, and improved message conveyance to the audience.


## Usability Test of the System

Utilizing usability testing tasks, subjective scales, and user feedback, we identify usability issues, informing the direction for system design optimization iterations to enhance the overall user experience.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_imgs/gnvis/gnvis/15.jpg" title="DUIIT image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     SUS scale score statistics.
</div>

Experimental results were analyzed using Excel and SPSS. Statistical analysis of subjective scale data and task completion revealed a high Cronbach alpha coefficient of 0.876, signifying the reliability of the data. The total system SUS score, presented in Table 5, is 82.78, indicating a high usability level for the proposed animated advertising poster generation system.


# Discussion
In this research paper, we propose an innovative method and tool for generating animated posters, enhancing existing online design platforms. We investigate the design influencing factors of animated advertising posters, focus on stylized animated effects, construct a semantic matching model of animated style, summarize the poster design strategy, and build a parametric generation model of animated advertising posters. In the design practice, a prototype of animated advertising poster generation tool targeting small and medium-sized businesses and junior designers is designed and developed based on the design thinking approach, and the validity and system usability of the model is verified by testing.

**The key contributions of this paper are as follows:**

**1. Animated Style Evaluation Model:**

- Established a comprehensive five-dimensional model for animated style evaluation.
- Developed a style labeling system using the funnel model, incorporating semantic vocabulary collection, cleaning, clustering, screening, optimization, and verification.
- Generated a dynamic elements structure by deconstructing fundamental element attributes and gathering prevalent dynamic effects, and formed a dynamic style labeling dataset through the creation of dynamic samples and the collection of style labels.
- Trained a BP neural network model for animated style prediction and built a style-matching model using a genetic algorithm for two-way matching of animated effects and style semantics.

**2. Parametric Generation Model of Animated Advertising Posters:**
- Proposed a parametric generation model by integrating the dynamic style-matching model and planned the technical route and completed the prototype implementation.
- Validated the model through comparison experiments for effect evaluation, subjective quality evaluation, and memory tests.

**3. Design Practice and User Evaluation:**
- Conducted design practice and user evaluation using the design thinking approach.
- Investigated user pain points and needs, clarified the system architecture, and constructed a feasible technical route and refined the design



