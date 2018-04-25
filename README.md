# March_Madness_2018
One Task:
* Predict outcomes of all possible match-ups in the 2018 NCAA Division I Men’s Basketball Championships

## Motivation
It has once again that time of year, the hottest sport championship is here. Many teams (and also fans) are aiming for the top. As a hired bracketologist (ok, that may not be a real profession but there is such a thing called bracketology so who knows maybe one day), your job is to predict the probabilities of every single match up for every team in this years March Madness competition. 

Submissions are scored on the log loss:

![log loss](https://cdn-images-1.medium.com/max/1600/1*RQ896sPBSAgMqq3ya9V2CA.png) 

where

n is the number of games played
y^i is the predicted probability of team 1 beating team 2
yi is 1 if team 1 wins, 0 if team 2 wins
log() is the natural (base e) logarithm

## Data
The data can be found in the [2018 Men's NCAA Basketball March Madness](https://www.kaggle.com/c/mens-machine-learning-competition-2018) kaggle competition. There are over 25 different data frames to work with, one needs to be careful when merging the data together.

## Methods
Feature Engineering:
* Created new features based on the big [Four Factors](https://www.basketball-reference.com/about/factors.html) that determine how good a team plays

Machine Learning models:
* Random Forest Classifier
* Adaboost classifier ensembling with Decision Tree Classifier
* XGBoost Classifier
* Voting Classifier

## Findings
My conclusion is that this task is nearly impossible because there are so many factors to consider. Also, as someone who has never watched a full college basketball game, I needed to do a lot of research to understand which features were important. I look forward to next year's competition. 

Also, I have suspicions of an NCAA Basketball Coach Cartel conspiracy, but that's for another project.
