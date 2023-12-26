# A-Comparative-Analysis-of-European-City-Police-Presence-on-Twitter
Master Thesis 2023 EPFL
Shasha Jiang

This repostoy is for master thesis with title "A Comparative Analysis of European City Police Presence on Twitter"

## Abstract
---
This study comprehensively analyses 21 Twitter accounts from city police departments across 16 European cities. It examined various communication practices exhibited by city police Twitter accounts, including post frequency and timing, retweet tendencies, resource-sharing strategies, language use, and hashtag employment. The research also investigated city police-related tweets from citizens in April and May 2023, providing a comparative perspective on topic preferences between police departments and citizens. Although common characteristics emerged among police accounts, each city displayed specific focal topics. Generally, the areas of concern for both citizens and police overlapped, but they emphasized different events and perspectives. 

## Structure
---
### [01] documentation
Here is the thesis itself saved as the `report.pdf` and the thesis denfense slieds `presentation.pdf`. 

### [02] notebooks

In notebook are all codes used for thesis for data collection, data prepocess and analysis with plots making and topic modelling. The excution order is:

- tweets_collection.ipynb: Collecting tweets with Twittwer API, with API keys stored in `[03]data/collected\_twitter/keys`
- plots_4-6.ipynb: Making plots in chapter 4, chapter 5 and chapter 6
- context_analysis_7.ipynb: Topic modelling and sentimental anlysis for chapter 7

### [03] data

*this folder is a structure to run the code, the real data store in this [link](...)
Stored all data for notebooks.
 - collected_twitter:  orginal collected twitter from API
 - tweets: categorizes and prepossed tweets used by analysis and modelling 

### [04] account_informations

Basic information collected for twitter accounts, inculding:
accounts handler name and city, accounts followers and created date, city population etc.

### [05] analysis_result

The result from analysis stored here, 
- plots: all plots used in the report. 
- senti_res3_acount,sent_res3_search: sentimental analysis result of account and search tweets.
- BERTopics2: result of bertopic model.

## Usage
---


## Repository Tree
---



