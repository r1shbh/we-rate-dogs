# we-rate-dogs
A project by Udacity's Data Analyst Nanodegree to gather data via web scraping from twitter, assessing and cleaning the data.

## About files:
- `twitter-archive-enhanced.csv`: Given archived dataset for dog ratings scraped via tweet
- `wrangle_act.ipynb`: The Jupyter notebook consisting of all Data Wrangling steps
- `wrangle_report.html`: The final report in slides format of the `wrangle_act.ipynb`
- `twitter_archive_master.csv`: Final cleaned tweets with all databases combined (containes no retweets or replies)
- `final_retweets.csv`: Final cleaned retweets
- `final_replies.csv`: Final cleaned replies
- `tweet_json.csv`, `tweet_json.txt` and `image-predictions.tsv` created in intermediate steps of Data Gathering
- `analysis.ipynb`: Jupyter notebook consisiting of basic initial analysis of the final `twitter_archive_master.csv`
- `act_report.html`: The final report in slides format of `analysis.ipynb`

## Libraries used:
- numpy
- pandas
- matplotlib
- seaborn
- requests
- tweepy
- os
