# A Comparative Analysis of European City Police Presence on Twitter
Master Thesis 2023, EPFL
Shasha Jiang

This repository is for the master thesis titled "A Comparative Analysis of European City Police Presence on Twitter."

## Abstract
---
This study comprehensively analyzes 21 Twitter accounts from city police departments across 16 European cities. It examines various communication practices exhibited by city police Twitter accounts, including post frequency and timing, retweet tendencies, resource-sharing strategies, language use, and hashtag employment. The research also investigates city police-related tweets from citizens in April and May 2023, providing a comparative perspective on topic preferences between police departments and citizens. Although common characteristics emerged among police accounts, each city displayed specific focal topics. Generally, the areas of concern for both citizens and police overlapped, but they emphasized different events and perspectives.

## Structure
---
### [01] documentation
Here is the thesis itself saved as the `report.pdf` and the thesis defense slides `presentation.pdf`.

### [02] notebooks

In the notebook are all the codes used for the thesis for data collection, data preprocessing, and analysis with plot-making and topic modeling. The execution order is as follows:

- `tweets_collection.ipynb`: Collecting tweets with the Twitter API, with API keys stored in `[03]data/collected_twitter/keys`.
- `plots_4-6.ipynb`: Making plots in chapters 4, 5, and 6.
- `context_analysis_7.ipynb`: Topic modeling and sentimental analysis for chapter 7.

### [03] data

*This folder is a structure to run the code; the real data is stored at this [link](...).*
Stored all data for notebooks.
 - `collected_twitter`: original collected Twitter data from API.
 - `tweets`: categorized and preprocessed tweets used for analysis and modeling.

### [04] account_information

Basic information collected for Twitter accounts, including:
account handler name and city, account followers and creation date, city population, etc.

### [05] analysis_result

The results from the analysis are stored here:
- `plots`: all plots used in the report.
- `senti_res3_account`, `sent_res3_search`: sentimental analysis results of account and search tweets.
- `BERTopics2`: result of the BERTopic model.

## Usage
---
Get real data at [link](...) and run code in notebooks with the results saved in `analysis_result`.


## Repository Tree
```bash
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
```