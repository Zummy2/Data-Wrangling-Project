# Introduction
Real-world data rarely comes clean. Using Python and its libraries, I will gather data from a variety of sources and in a variety of formats, assess its quality and tidiness, then clean it. This is called data wrangling. I will document your wrangling efforts in a Jupyter Notebook, plus showcase them through analyses and visualizations using Python (and its libraries).

## Project Overview
The tasks i will be carrying out in this project are as follows:

- Step 1: Gathering data

- Step 2: Assessing data

- Step 3: Cleaning data

- Step 4: Storing data

- Step 5: Analyzing and visualizing data

- Step 6: Reporting

## Datasets
The dataset that I will be wrangling (and analyzing and visualizing) is the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international media coverage.

Also The tweet image predictions dataset,this file (image_predictions.tsv) is present in each tweet according to a neural network. 

Finally, additional data from the Twitter API, I will gather each tweet's retweet count and favorite ("like") count at the minimum and any additional data I find interesting. Using the tweet IDs in the WeRateDogs Twitter archive,I will query the Twitter API for each tweet's JSON data using Python's Tweepy library and store each tweet's entire set of JSON data in a file called tweet_json.txt file.

Each tweet's JSON data will be written to its own line. Then I will read this .txt file line by line into a pandas DataFrame with (at minimum) tweet ID, retweet count, and favorite count.