# StarBucks-Promotional-Offer-Recommendation
This is a capstone project for the course completed in response to Udacity- Data Scientist Nanodegree Program.   
Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks.
Not all users receive the same offer, and that is the challenge to solve with this data set.   
Main task is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type.
You can find the blog post link here [MEDIUM-BLOG](https://nimishsoni.medium.com/promotional-offer-recommendation-engine-for-starbucks-coffee-48bc6d0a1988)


## Motivation
The motivation behind this project was exploring the Starbuck’s Dataset which simulates how people make purchasing decisions and how those decisions are influenced by promotional offers.   
It was driven by following questions that were answered as the project came to its completion:
* What is the proportion of clients who have completed the offers based on gender, age, and income levels?
* What is the Best supervised learning model for predicting offers based on demographic data?
* What are the most important features that help drive the offers in customers?

## Summary 
The project was completed in the following phases:
* Dataset Exploration and Preprocessing:- In this process, the data provided was cleaned, processed and merged for further analysis.
* Data Analysis &  Visualization: In this process, few questions were answered by analysing the question and  providing visualization which answers the question 1:     
* Building supervised Model and Performance Evaluation: In this step, various machine learning model(Decision Tree, Gaussian NB and Random Forest) were tested on the given dataset and their respective performances were evaluated. This step also answers Question 2. 
* Top Feature Selection: In this process, the best estimator among the three was used to predict the most important feature that impacted the promotional offer completion in customers.   

## File Descriptions
#### Data Dictionary
##### profile.json
Rewards program user profile (17000 users x 5 fields)

gender: (categorical) M, F, O, or null   
age: (numeric) missing value encoded as 118   
id: (string/hash)   
became_member_on: (date) format YYYYMMDD   
income: (numeric)      

##### portfolio.json
Offer details sent during 30-day test period (10 offers x 6 fields)

reward: (numeric) money awarded for the amount spent   
channels: (list) web, email, mobile, social   
difficulty: (numeric) money required to be spent to receive reward   
duration: (numeric) time for offer to be open, in days   
offer_type: (string) bogo, discount, informational   
id: (string/hash)     
 
##### transcript.json
Transaction logs (306648 events x 4 fields)

person: (string/hash)   
event: (string) offer received, offer viewed, transaction, offer completed   
value: (dictionary) different values depending on event type   
offer id: (string/hash) not associated with any "transaction"   
amount: (numeric) money spent in "transaction"   
reward: (numeric) money gained from "offer completed"   
time: (numeric) hours after start of test   

## Prerequisites
* Python
* VsCode
* Jupyter Notebook
* Pandas
* Numpy
* Matplotlib
* Seaborn
* Json
* Sklearn model selections
* Sklearn.metrics 
* Matplotlib patches
* os
* sys
* Sklearn tree, Naive bayes, ensemble
* itertools


## Acknowledgement
I would like to thank Udacity for the project, and Starbucks for providing the data.
