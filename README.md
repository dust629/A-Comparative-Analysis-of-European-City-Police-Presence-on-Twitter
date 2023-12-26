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
Get real data in [link](...) and run code in notebooks with result saved in `analysis_result`

## Repository Tree
.
├── account_information
├── analysis_result
│   ├── BERTopics2
│   ├── plots
│   ├── senti_res3_account
│   └── senti_res3_search
├── data
│   ├── collected_twitter
│   │   ├── added_account_tweets
│   │   ├── added_search_tweets
│   │   ├── keys
│   │   └── profile
│   └── tweets
│       ├── all_account_city
│       ├── all_search_city
│       ├── all_search_city21
│       ├── filter_search
│       ├── processed_account_tweets
│       ├── processed_search_tweets
│       ├── topically_processed_account_tweets
│       ├── topically_processed_search_tweets
│       ├── translated_account_city
│       └── translated_search_city
├── documentation
│   ├── account-select-flow.png
│   ├── presentation.pdf
│   ├── report.pdf
│   └── search-tweets-select-flow.png
├── notebooks
│   ├── context_analysis_7.ipynb
│   ├── plots_4-6.ipynb
│   └── tweets_collection_preprocess.ipynb
└── README.md
