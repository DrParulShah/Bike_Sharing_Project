# Bike Sharing Assignment
# submitted by Parul Shah

## INTRODUCTION
Bike Sharing Assignment tends to identify the factors affecting the demand for these shared bikes in the American market

Table of Contents


Acknowledgements

## Table of Contents
* Problem statement and Goal
* Overview of Data Analysis Approach
* Summary of Analysis
* Acknowledgements


## Problem statement and Goal
A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic finding it hard to sustain .
Company aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19.

Goal : Identify the factors affecting the demand for these shared bikes in the American market

Dataset : day.csv

## Overview of Data Analysis Approach
The model was trained using two approaches:
1. varaible selection using RFE + manual dropping of variables based on p-value and VIF
2. adding all variables to start with and then drop them one at a time based on VIF and p-values

Model performance was analyzed based on R2, adjusted R2 and F Statistics.
Residual analysis and assumtions verification was also done.
Hypothesis testing too was conducted.

## Summary of Analysis
Which variables are significant in predicting the demand for shared bikes ? 
Based on Model analysis, below variables are significant: yr, workingday, temp, windspeed, season2, season4, mnth9, weekday6, weathersit2 and weathersit3. 
Some variables will impact in positive way while others will have negative impact. 

Interpretation of Coefficients (in decreasing order of significance):

1. temp: A coefficient value of ‘0.5636’ indicates that a unit increase in temp variable, increases the bike hire numbers by 0.5636 units (almost 56% hike in count whhich makes sense loggically too)

2. yr: A coefficient value of ‘0.2308’ indicates that a unit increase in yr variable, increases the bike hire numbers by 0.2308 units (which is almost 23% hike in count). This indicates that with time, popularity of bike is increasing which in turn increases the count

3. weathersit_3: A coefficient value of ‘-0.3070’ indicates that, a unit increase in Weathersit3 variable, decreases the bike hire numbers by 0.3070 units (30% reduction in count)

4. season_4: A coefficient value of ‘0.128744’ indicates that a unit increase in season_4 variable increases the bike hire numbers by 0.128744 units (12% rise in count)

5. windspeed: A coefficient value of ‘-0.155191’ indicates that, a unit increase in windspeed variable decreases the bike hire numbers by 0.155191 units (~15% reduction in count whhich makes sense loggically too)

6. workingday: A coefficient value of ‘0.043203’ indicates that a unit increase in workingday variable increases the bike hire numbers by 0.043203 units (a hike of ~4%)

7. season_2: A coefficient value of ‘0.082706’ indicates that a unit increase in season_2 variable decreases the bike hire numbers by 0.082706 units (a rise of ~ 8%)

8. mnth_9: A coefficient value of ‘0.094743’ indicates that a unit increase in mnth_9 variable increases the bike hire numbers by 0.094743 units (a rise of ~9.4%)

9. weekday_6: A coefficient value of ‘0.056909’ indicates that a unit increase in weekday_6 variable increases the bike hire numbers by 0.056909 units (a rise of ~5.6%)

10. weathersit_2: A coefficient value of ‘-0.074807’ indicates that a unit increase in Weathersit2 variable, decreases the bike hire numbers by 0.074807 units (~7.4% reduction in count)

11. const: The Constant value of ‘0.084143’ indicates that in the absence of all other predictor variables (i.e. when x1,x2...xn =0), The bike rental can still increase by 0.084143 units (~8.4% rise in count)

## Technologies Used
* Anaconda3 
* jupyter 
* Notebook
* python 3.9

## Acknowledgements
Thanks to Upgrad Instructors and Live Sessions

## Contact
Created by [@DrParulShah] - feel free to contact me!


