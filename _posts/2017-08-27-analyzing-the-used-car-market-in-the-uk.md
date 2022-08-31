---
layout: post
title: "Analyzing the Used Car Market in the UK- SQL and Data Warehousing "
author: "Ross Lancaster"
categories: facts
tags: [sample]
image: cars.jpg
---

Whether you are a manufacturer, dealer, or a consumer, knowing which aspects of a used car contribute to a high resale value can be crucial information. Thus, I utilized multiple datasets compiled by researchers at the University of Glasgow detailing numerous aspects of the used car market in the UK in order to better understand the trends behind used car values. After data quality checks and cleaning the data, these datasets were uploaded to Microsoft SQL Server. A data warehouse comprising three fact tables and eight dimension tables was created. The entity-relationship diagram for the data warehouse is provided below. 

![Entity Relationship Diagram](/assets/entity.JPG)

After the successful creation of the data warehouse, the data was exported to Excel for analysis. A dashboard was creating utilizing pivot charts and macros for easy analysis of the trends behind used car values. This analysis resulted in several observations including the following:

* Used car prices decrease with every mile driven, every additional seat, and every additional door but increase with each year newer the registration year is
* Less traditional car colors occupy both extremes of average used car prices while more traditional colors have average prices in the middle
* Hatchbacks, the most common body type, have the second lowest average used car price
* Specialty vehicles like campers and limousines have the highest average used car prices
* Used car prices tend to increase in the colder months and decrease in the warmer months
* Cars with more ecofriendly fuel sources tend to have higher used car prices
* Cars with manual transmission have the lowest average used car prices with semi-automatic cars having prices over ten times higher on average
* McLaren is the make with the highest average used car price and Daewoo is the make with the lowest average used car price
* Many of the top and bottom 10 makes for list price are also found in the top and bottom 10 for used car price
* Sales for the top 10 selling manufacturers tended to increase every year from 2011 to 2019 before plummeting in 2020
* Luxury and sports car brands tended to have the highest resale values while more budget friendly brands had the lowest resale values

The files used to create the data warehouse can be found [here](https://github.com/rosslancaster1/Car-Data-Warehouse).
