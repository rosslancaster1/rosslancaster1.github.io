---
layout: post
title: "Predicting Household Poverty in Costa Rica"
author: "Ross Lancaster"
categories: facts
tags: [sample]
image: costarica.JPG
---

As there is only a finite amount of aid money available, it is important to determine who would benefit from this assistance the most. This is a problem currently facing areas like Costa Rica where many citizens are living in poverty. One main challenge is that it is difficult for those in the lowest economic brackets to report their financial situations to the proper authorities. Thus, alternative methods of determining who requires social assistance are needed in order to more effectively distribute aid to those who need it most. One such alternative method is the Proxy Means Test (PMT) that looks at factors such as the materials used to construct a house and the assets within the house to determine how much aid that household requires. This is where machine learning can be a very powerful tool as it can be used to increase the accuracy of the PMT. 

The Inter-American Development Bank provided a dataset where each row represents a different individual in Costa Rica. Each row also had a multitude of features that describe the individual’s household ranging from the material used to make the house’s walls to if someone in the house owns a tablet. These features were used to make models to predict the class label for each individual. The class labels for this dataset are ordinal integers ranging from 1 to 4, with 1 indicating the individual’s household is in “extreme poverty” and 4 indicating “nonvulnerable households.” As the dataset included a multitude of features, many of them required preprocessing before models could be constructed.

Extensive data cleaning, feature creation, and feature selection were performed prior to creating any models. For example, some features that took on a wide range of values had to be standardized so that they would not dominate the predictions over the many binary features. Also, multiple features describing the condition of the household's floors were combinedto help with dimensionality reduction. Finally, it was eventually decided to only include the features that had the strongest correlation with the class label in the analysis.

An MLP classifier, random forest classifier, and a logistic regression model were built in order to analyze the data. Analysis was run both with and without principal component analysis. As the classes were unbalanced, F-score was used to quantity the performance of the models because it combines both recall and precision. The random forest classifier resulted in the highest F-score while the logistic regression modeled resulted in the lowest F-score. Thus, the random forest classifier and the logistric regression model were the most and least accurate models, respectively.

This project was completed in Python and its code can be found [here](https://colab.research.google.com/drive/1ZXG83NT6VEb8VHxbYRP4bOYSzx-VJ0B6?usp=sharing).
