---
layout: post
title: "RPI Datathon- Utilizing Mobile Advertising Data "
author: "Paul Le"
categories: facts
tags: [sample]
image: datathon.JPG
---

During my final semseter of graduate school my entire department took part in a datathon hosted by RPI. We were provided with mobile advertising data from a corporate sponsor and tasked with creating a way to predict when demand-side platforms would make a bid for a mobile advertising spot. I chose to tackle this problem by using to Python to create XGBoost and LightGBM models that were able to predict when these bids would occur. Extensive feature creation and selection was necessary. For example, many categorical varaibles had to be converted to dummy variables. Due to privacy concerns, this code cannot be shared publically. 

Another portion of this project was recognizing that over 95% of instances do not result in a bid. Thus, a stratified sample was taken in order for the models to be able to accurately learn the factors that separate a successful bid from an unsuccesful one. This also played a large part in selecting boosting algorithms for the models. Overall, after stratifying the sample both models were able to predict whether or not a bid would be made with over 80% accuracy. However, the XGBoost model demonstrated a slighly higher performance. I also attempted to utilize PCA on this dataset but the results did not show any improvement. 

After creating the models I submitted them alongside a technical report and analysis on how my solution would help the mobile advertising company's business. I was selected as one of the five finalists and presented my results and the theory behind them to a panel of judges. Ultimately, the judges chose my project as the first place winner and recipient of the $1500 prize. Notably, I was the only team of one to be selected as a finalist and won over teams of 4-5 members. 
