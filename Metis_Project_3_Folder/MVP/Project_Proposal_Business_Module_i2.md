# Project Proposal Business Module (iteration 2)

### `The Question`

Since the onslaught of the COVID pandemic, predicting covid caseload in the US has been relatively difficult with disjoint information arising from all directions. Thus, the federal government has had to toil to sort the barrage of information into a unified image. 

I will use twitter sentiment to better predict COVID caseload. My first proposed solution path is to build a natural language processing model to perform a topic analysis on twitter sentiment, and combine that with a time-series analysis of COVID caseload in the United States. 

The desired impact of this project is to develop a model that might predict areas of concern for future outbreaks based on twitter sentiment in real time. Doing so would ensure resources are reaching the right places in order to combat viral outbreaks before they spread far and wide. The impact hypothesis is that building a predictive NLP model to analyze twitter sentiment will improve the time it takes to allocate resources (and perhaps the degree of resource allocation). This hypothesis assumes that using twitter will be a good indicator of caseload, which may not be true.  

### `Data`

For the preliminary exploratory data analysis (EDA), I plan to use two datasets.

The first dataset is a dataset of tweets (International) cataloged on the website _Kaggle_ as a text classification challenge. It is open source (provided you have an account for _Kaggle_) and can be found here: https://www.kaggle.com/datatattle/covid-19-nlp-text-classification. The raw data consists of nearly 3800 rows and 6 columns. Each row represents an individual tweet and the columns include UserName (enumerated as a list of numbers for privacy), ScreenName (same as UserName?), Location (city where tweet was sent), TweetAt (date that tweet was sent), OriginalTweet (the Tweet itself), and Sentiment.

The second dataset is a time-series dataset of COVID cases and deaths (in the United States only) provided by Johns Hopkins. It is also open source and can be found here: https://www.kaggle.com/codebreaker619/john-hopkins-covid-19-case-tracker-dataset. The raw data consists of nearly 20000 rows and 13 columns. each row is the number of new Covid cases reported in a given day at a city-level location. The columns for this dataset include state, date, total population, cululative cases, cumulative cases per 100000, cumulative deaths, cumulative deaths per 100000, new cases, new cases 7 day rolling average, new deaths, new deaths 7 day rolling average, new deaths per 100000, and new cases per 100000.

### `Tools`

- Google sheets for data manipulation

- Tableau for data visualization

### `MVP Goal`

My MVP goal is to create a well-defined iteration of my project proposal, along with some visualizations pertaining to twitter sentiment and COVID caseload. 

### `Next Steps`

- choose approriate subset of COVID caseload data that can match with cleaned Twitter data 
- join (filtered) datasets on location and date
- plot line of cumulative cases over time and see how sentiment evolves as cases grow (with fixation on areas where COVID case growth is steep vs. shallow)