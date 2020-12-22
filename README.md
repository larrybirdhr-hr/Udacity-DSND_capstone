# Udacity-DSND_capstone
This repository is to host the Udacity Capston project. The Starbucks projected is selected. Udacity inclass workspace is used to complete this project

## Project Overview
This data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks. The task is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type. 

The motivation of this project is to provide insight for the company advertisement strategy to help the company improve the  efficiency by sending offers to targeted customers. 

One conclusion from this study is that the customer membership duration is the dominant factor for a successful offer response. This will be detailed in the result and discussion. 

## Libraries and Dependencies

* This workbook can be ran using Python versions 3.*.

* Stardard Python libraries for Machine Learning: NumPy, Pandas, Math, Datetime, Sciki-Learn.

* Data Visualization librraries: Matplotlib, Seaborn.

## Data Files

The data is contained in three files:

* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

**portfolio.json**
* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)

**profile.json**
* age (int) - age of the customer 
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

**transcript.json**
* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record

## Instructions
* The Starbucks_Capstone_notebook.ipynb is self contained and should run automatically.
* The 3 data files mentioned above need to be located in the data folder. 

## Acknoledgement
This project is to partial fullfillment of Udacity Data Scientist Nanodegree. The data set is simulated data provided by the Starbucks. 

## Results and Discussion
Results and detailed discussion are published [here](https://medium.com/@huangr76/a-predictive-modeling-for-starbucks-offer-response-538ade0d042a). 
