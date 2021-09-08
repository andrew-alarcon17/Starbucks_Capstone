# Starbucks Capstone Project

## Project Description
This project contains mimicked user behavior on the Starbucks rewards mobile application. In this app, Starbucks sends out offers to its customers, like BOGO (buy one, get one free) or a discount. Different users get different offers. So the main goal of this project was to figure out which offers succeed the most to which types of customers.

## About the Data

### Portfolio
The porfolio dataset contains information on the offers, such as:

* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)

### Profile
The profile dataset contains information about the customer, such as:

* age (int) - age of the customer 
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

### Transcript
The transcript dataset contains information about what kind of activity was performed on an offer, such as:
* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record

## Findings

Here are a few findings after cleaning and combining the necessary dataframes in order to figure out which offers were successful to which users.

<img src="https://github.com/andrew-alarcon17/Starbucks_Capstone/blob/main/Charts/Successful%20Bogo%20by%20Age.png" width="500">

Here we see that the BOGO offer in red is the most successful to these 4 age groups.

<img src="https://github.com/andrew-alarcon17/Starbucks_Capstone/blob/main/Charts/Successful%20Discount%20by%20Age.png" width="500">

Here we see the informational offers are most successful with seniors and adults.

<img src="https://github.com/andrew-alarcon17/Starbucks_Capstone/blob/main/Charts/Successful%20Info%20by%20Age.png" width="500">

For discounts, the ones in blue and purple dominate in all 4 age groups.

## Acknowledgements
This data was provided by the Udacity Data Science Course team.



