#Project Proposal Business Module

##`The Question`

Since the onslaught of the COVID pandemic, a proper allocation of resources based on covid caseload has been poorly automated with disjoint information arising from all directions without being put in context. Thus, US state and federal governments have had to toil to sort the barrage of information into a unified image. 

The question I wish to address is: can we better automate the process of resource allocation by utilizing twitter sentiment? My first proposed solution path is to build a natural language processing model to perform a topic analysis on twitter sentiment, and combine that with a time-series analysis of COVID caseload in the United States. 

The desired impact of this project is to more efficiently allocate resources so that resources are not wasted excess of some predefined baseline amount. The impact hypothesis is that automating the process of resource allocation using a ubiquitous tool like twitter as an engine will improve both the time it takes to allocate resources, as well as eliminating superfluous allocation. The hypothesis assumes that using twitter will be a good indicator of caseload, which may not be the case.  

(I need to plunge more time into research on metric for determining successful resource allocation in order to verify the model)

##`Data`

For the preliminary exploratory data analysis (EDA), I plan to use two datasets.

The first dataset is a dataset of tweets (International) cataloged on the website _Kaggle_ as a text classification challenge. It is open source (provided you have an account for _Kaggle_) and can be found here: https://www.kaggle.com/datatattle/covid-19-nlp-text-classification. The raw data consists of nearly 3800 rows and 6 columns. Each row represents an individual tweet and the columns include UserName (enumerated as a list of numbers for privacy), ScreenName (same as UserName?), Location (city where tweet was sent), TweetAt (date that tweet was sent), OriginalTweet (the Tweet itself), and Sentiment.

The second dataset is a time-series dataset of COVID cases and deaths (in the United States only) provided by Johns Hopkins. It is also open source and can be found here: https://www.kaggle.com/codebreaker619/john-hopkins-covid-19-case-tracker-dataset. The raw data consists of nearly 20000 rows and 13 columns. each row is the number of new Covid cases reported in a given day at a city-level location. The columns for this dataset include state, date, total population, cululative cases, cumulative cases per 100000, cumulative deaths, cumulative deaths per 100000, new cases, new cases 7 day rolling average, new deaths, new deaths 7 day rolling average, new deaths per 100000, and new cases per 100000.



##`Tools`

-Google sheets for data manipulation

-Tableau for data visualization



##`MVP Goal`

My MVP goal is to create a well-defined iteration of my project proposal, along with some visualizations pertaining to twitter sentiment and COVID caseload. 