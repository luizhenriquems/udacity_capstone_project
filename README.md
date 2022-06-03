# # Udacity Capstone Project

## Project Context

The main idea of the project was to analyze the provided data and develop a model that indicates an offer for a specific customer. The given dataset simulate a simplified version of data regarding customer behaviour on the Starbucks mobile app. Frequently, Starbucks sends out offers to app mobile users through different channels. It can be classified in ‘buy one get one free’ (BOGO), discounts — when a user receives a reward equal to a fraction of the amount spent — and an informational offer.

## Used Libraries

pandas
numpy
math
json
datetime
pickle
matplotlib
seaborn

## Dataset

The data set contains three files:

Portfolio: it describes the characteristics of each offer, including its duration and the amount a customer needs to spend to complete it (difficulty).
Profile: it has customer demographic data including their age, gender, income, and when they created an account on the Starbucks rewards mobile application.
Transcript : it describes customer purchases and when they received, viewed, and completed an offer. An offer is only successful when a customer both views an offer and meets or exceeds its difficulty within the offer’s duration.

## Dataset Schemas

portfolio.json
  id (string) — offer id
  offer_type (string) — type of offer ie BOGO, discount, informational
  difficulty (int) — minimum required spend to complete an offer
  reward (int) — reward given for completing an offer
  duration (int) — time for offer to be open, in days
  channels (list of strings)

profile.json
age (int) — age of the customer
became_member_on (int) — date when customer created an app account
gender (str) — gender of the customer (note some entries contain ‘O’ for other rather than M or F)
id (str) — customer id
income (float) — customer’s income

transcript.json
event (str) — record description (ie transaction, offer received, offer viewed, etc.)
person (str) — customer id
time (int) — time in hours since start of test. The data begins at time t=0
value — (dict of strings) — either an offer id or transaction amount depending on the record

## File Description

- Starbucks_Capstone_notebook.ipynb

- data:
  -portfolio.json
  -profile.json
  -transcript.json

- README.md


## Results

You can find the main insights in this post [here](https://medium.com/@luizhenriquems/starbucks-mobile-app-exploring-the-engagement-675007ab80ae)
