# Data Wrangling Project
A project by Udacity's Data Analyst Nanodegree to gather data via web scraping from twitter, assessing and cleaning the data.

## Project Details
#### Tasks in this project are as follows:

Data wrangling, which consists of:
1. Gathering data (downloadable file in the Resources tab in the left most panel of your classroom and linked in step 1 below).
2. Assessing data
3. Cleaning data
4. Storing, analyzing, and visualizing the wrangled data
5. Reporting on 1) your data wrangling efforts and 2) your data analyses and visualizations

### 1. Gathering Data for this Project
Gather each of the three pieces of data as described below in a Jupyter Notebook titled `wrangle_act.ipynb`:

- **The WeRateDogs Twitter archive**: Already given as `twitter_archive_enhanced.csv`

- **The tweet image predictions**: i.e., what breed of dog (or other object, animal, etc.) is present in each tweet according to a neural network. This file (image_predictions.tsv) is hosted on Udacity's servers and should be downloaded programmatically using the Requests library and the following URL: https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv

- **Each tweet's retweet count and favorite ("like") count at minimum, and any additional data you find interesting**: Using the tweet IDs in the WeRateDogs Twitter archive, query the Twitter API for each tweet's JSON data using Python's Tweepy library and store each tweet's entire set of JSON data in a file called tweet_json.txt file. Each tweet's JSON data should be written to its own line. Then read this .txt file line by line into a pandas DataFrame with (at minimum) tweet ID, retweet count, and favorite count.


### 2. Assessing Data for this Project
After gathering each of the above pieces of data, assess them visually and programmatically for quality and tidiness issues. Detect and document at least eight (8) quality issues and two (2) tidiness issues in your `wrangle_act.ipynb` Jupyter Notebook.

### 3. Cleaning Data for this Project
Clean each of the issues you documented while assessing. Perform this cleaning in `wrangle_act.ipynb` as well. The result should be a high quality and tidy master pandas DataFrame (or DataFrames, if appropriate).

### 4. Storing, Analyzing, and Visualizing Data for this Project
Store the clean DataFrame(s) in a CSV file with the main one named twitter_archive_master.csv. If additional files exist because multiple tables are required for tidiness, name these files appropriately. Additionally, you may store the cleaned data in a SQLite database (which is to be submitted as well if you do).

### 5. Analyze and visualize your wrangled data
Done in `analysis.ipynb` Jupyter Notebook. At least three (3) insights and one (1) visualization must be produced.

## Reporting for this Project
- Create a 300-600 word written report called `wrangle_report.html` that briefly describes your wrangling efforts. This is to be framed as an internal document.

- Create a 250-word-minimum written report called `act_report.html` that communicates the insights and displays the visualization(s) produced from your wrangled data. This is to be framed as an external document, like a blog post or magazine article, for example.

Both of these documents can be created in separate Jupyter Notebooks using the Markdown functionality of Jupyter Notebooks, then downloading those notebooks as PDF files or HTML files (see image below). You might prefer to use a word processor like Google Docs or Microsoft Word, however.

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
