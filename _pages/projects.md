---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

This page showcases the projects I have led and collaborated on, along with their results.


## Project 1: GEDI and Landsat-8 Data Fustion Using Machine Learning
This project quantified biomass loss due to saltwater intrusion in Wicomico, Somerset, and Dorchester counties, Maryland. The GEDI L4A biomass product served as the dependent variable in a random forest regression model, with Landsat-8 bands as independent variables. Landsat-8 data for the study area were collected using the Google Earth Engine platform. The trained model produced wall-to-wall biomass maps for 2013 and 2021. The following figure presents the results: (A) Landsat-8 composite of the study area, (B) GEDI data, (C) estimated biomass map for 2013, and (D) estimated biomass map for 2021. The codes for this project are available on my [GitHub repository](https://github.com/mo-agh/GEDI-Landsat_data_fusion).

![project1](/images/projects/project1_final.png)


## Project 2: LiDAR Canopy Height Outlier Detection
In this project, I developed a machine learning framework to detect outliers in canopy height estimates from GEDI LiDAR data. The model was a multimodal convolutional neural network that utilized both GEDI data and ancillary data from NASADEM as input to predict whether GEDI canopy height estimates contained outliers. To generate the training dataset, LVIS LiDAR data was used as ground truth. Additionally, a SHAP analysis was performed to identify the most influential input features affecting the model’s predictions. The following figure presents some of the results: (A) a scatter plot of GEDI-LVIS crossovers used for generating the training dataset, (B) a true positive sample (red dots indicate the most influential SHAP features), and (C) a true negative sample. The codes for this project are available on my [GitHub repository](https://github.com/mo-agh/LiDAR_canopy_height_outlier_detection).

![project2](/images/projects/project2_final.png)


## Project 3: GEDI Gap Mapping
In this project, I created global maps of gaps in GEDI LiDAR data. The mapping was performed using Uber's H3 indexing system at resolutions 1 to 7, utilizing the GeoPandas and multiprocessing packages in Python. The following graphs show the global gap map and a zoomed-in view of an area in Africa. The codes for this project are available on my [GitHub repository](https://github.com/mo-agh/GEDI_gap_mapping).

![project3_!](/images/projects/project3_1.png)
![project3_2](/images/projects/project3_2.png)


## Project 4: LiDAR Ground Detection Enhancement
This project aimed to improve ground elevation estimation from GEDI LiDAR data. Ground elevations from LVIS LiDAR data were used as ground truth to train a convolutional neural network. The model incorporated NASADEM as ancillary data and reduced the RMSE of ground elevation estimates by 32 centimeters (8%). The following figure presents some of the model’s predictions, with grey, blue, and red lines representing GEDI, LVIS, and predicted ground elevations, respectively. The codes for this project are available on my [GitHub repository](https://github.com/mo-agh/improved_LiDAR_ground_detection).

![project4](/images/projects/project4.png)


## Project 5: Forest Canopy Height Change Detection
In this project, I quantified forest canopy height changes in Gabon from 2016 to 2023 using LiDAR data. The 2023 LiDAR data had ground-finding issues, which I corrected before the analysis. The scatter plots below illustrate the impact of this correction on the data. Additionally, canopy height changes were analyzed across five categories, with a mean and standard deviation of 0.7 meters and 3.7 meters, respectively, across all categories. The following map shows the changes in a small region of the study area. The codes for this project are available on my [GitHub repository](https://github.com/mo-agh/forest_canopy_height_change).

![project5_2](/images/projects/project5.png)

![project5_1](/images/projects/project5.gif)


## Project 6: LiDAR simulations from Point Cloud Data
This project focused on simulating GEDI LiDAR data using Airborne Laser Scanning (ALS) point cloud data. The simulator was set up with appropriate input parameters to generate 22-meter footprint waveforms. The following figure illustrates some of the results: on the left is the simulated GEDI waveform, which corresponds to the third footprint from the right on the map. The codes for this project are available on my [GitHub repository](https://github.com/mo-agh/ALS_simulation).

![project6](/images/projects/project6.png)


## Project 7: RTM Surrogate Model
In this project, I developed a framework to emulate the MODTRAN Radiative Transfer Model (RTM), which is widely used for atmospheric correction of optical satellite imagery. To achieve this, top-of-atmosphere (TOA) and bottom-of-atmosphere (BOA) spectroscopy data were used to train multiple machine learning models. The results showed that a deep learning autoencoder outperformed other models, achieving an R² of 98.23%, a 3.16% improvement over Random Forest. The following figure presents the visual results. The top left and top right panels display the best and worst estimation samples of the model, respectively. The bottom left panel illustrates error estimates, while the bottom right panel contains box plots of the performance metrics. This project resulted in a publication, which is available at [this link](https://www.mdpi.com/2673-4931/29/1/16).
The codes for this project are available on my [GitHub repository](https://github.com/mo-agh/RTM_surrogate_modeling).

![project7](/images/projects/project7.png)

