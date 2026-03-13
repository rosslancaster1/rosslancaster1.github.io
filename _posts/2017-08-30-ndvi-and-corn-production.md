---
layout: post
title: "NDVI and Corn Production"
author: "Ross Lancaster"
categories: facts
tags: [sample]
image: ndvi.jpg
---

This was a research project that I headed and worked in collaboration with NASA scientist Dr. Assaf Anyamba and researchers at the Oak Ridge National Laboratory. Python was chosen as the programming language for this project. 

NDVI is the normalized difference vegetation index and is a measure of the difference between infrared and near visible light that is reflecting off of Earth 
(NDVI = (NIR — VIS)/(NIR + VIS)). This allows one to quantify photosynthetic capacity as near infrared light is heavily reflected by the leaves of plants. In turn, one should be able to use NDVI data to make crop yield predictions. For this project we focused on corn as our crop of interest. Corn production statistics from the National Agricultural Statistics Service and NDVI data from NASA’s GIMMS Global Agricultural Monitoring(GLAM) system were utilized. Data was collected for the top five corn producing states, Iowa, Illinois, Nebraska, Minnesota, and Indiana, as well as from the top non-US corn producers in the world, China, Brazil, Argentina, and Ukraine.  Machine learning techniques such as linear regression, neural networks (multilayer perceptron), XGBoost, random forests, and K-nearest neighbor models were then used to determine the validity of the hypothesis that NDVI data should be able to predict corn production throughout the world.

Overall, 18 datasets in total were collected and cleaned to create the final dataframes. Extensive exploratory data analysis, feature selection/creation, and dimensionality reduction were completed as well. Finally, the machine learning models were created and deployed. The results indicated that the multilayer perceptron and random forest models are best suited for modeling the data. Their crop yield predictions exhibit error rates of less than 10%. On the other hand, the multivariate linear regression and K-nearest neighbors models displayed the worst results. Refining the models to better protect against overfitting would improve the results even further.

A sample of the code used for this project can be found [here](https://colab.research.google.com/drive/1z1cRPsLW668tl2kqmJbJiJRy-o3dCy_g?usp=sharing).
