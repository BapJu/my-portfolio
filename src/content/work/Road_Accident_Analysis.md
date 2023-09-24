---
title: Road Accident Analysis & IA Prediction Platform
publishDate: 2023-06-02 00:00:00
img: /assets/Road_Accident_Analysis.png
img_alt: Clustering of french accident
description: |
 Develop a comprehensive web platform that amalgamates Big Data, AI, and Web Development to catalog, analyze, and predict the severity of road accidents.
tags:
  - HTML / CSS / JS
  - PHP
  - IA models
---
## Overview

Road safety remains a significant concern worldwide. With the vast amount of data available regarding accidents, there lies an untapped potential to analyze and predict accident severities, thereby aiding in better road safety measures. This project strives to harness that potential, offering both a bird's eye view of past accidents and predictive insights into the severity of new incidents.

## Key Features

1. **Data Cleaning with RStudio**: 
    - Started with INSEE's dataset comprising over 75,000 road accidents from 2009 in France.
    - Cleaned to eliminate inconsistencies and transformed various parameters like age, vehicle description, road conditions, etc., into discrete values for enhanced analysis.

2. **AI-Powered Predictive Analysis**:
    - Utilized supervised and unsupervised machine learning models such as SVM, KNN, Random Forest, and MLP.
    - Analyzed the likelihood of accident severity based on diverse parameters.
    - Compared and ranked algorithms using metrics like the Silhouette Coefficient, Calinski-Harabasz Index, and the Davies-Bouldin Index.

3. **Interactive Web Platform**:
    - Creation of a site web with HTML5 & JS
    - Presented accidents on an interactive JS map for easy visualization.
    - Enabled addition of new accidents to the MySQL database through the web interface.
    - Integrated AI algorithms to predict and display the potential severity of any newly added accident in real-time.

4. **Backend Integration**:
    - Utilized PHP for backend operations, facilitating seamless communication with the MySQL database.

## Benefits

- **Informed Decision Making**: By visualizing past accidents and predicting the severity of new ones, authorities and individuals can make better-informed road safety decisions.
- **Efficient Data Handling**: With cleaned and optimized data, the platform ensures accurate predictions and clear visual representations.
- **Real-time Insights**: Immediate severity predictions for new accidents pave the way for timely interventions and improved safety protocols.

