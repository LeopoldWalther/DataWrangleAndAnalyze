# Wrangle and analyze data of WeRateDogs Twitter posts

This project is part of the Udacity Nanodegree Data Analyst. It is based on data
of the WeRateDog account. Main goal of this project is to follow through the
complete Data Analysis process. Firstly data is gathered from different sources:
 a local csv-file, a programmatically downloaded file and data downloaded via
 the twitter API. Secondly the data from the different sources is visually and programmatically assessed to be cleaned in the next step for the final
 analysis. The analysis compares the ratings, retweets and favorites of
 different dog stages and races.

## Quickstart
1. Install Anaconda, best with homebrew: `brew cask install anaconda `
2. To set path variable run : ```conda init```
3. Open Jupyter Notebookvwirh ```jupyter notebook```
4. In the notebook open the .ipyn-file.


## Structure

1. Gather: Data is gathered from three different sources of data as described
   in steps below:
   - The WeRateDogs Twitter archive. File twitter_archive_enhanced.csv as comma separated file in local directory.
   - The tweet image predictions, i.e., what breed of dog (or other object, animal, etc.) is present in each tweet according to a neural network. This file (image_predictions.tsv) is hosted on Udacity's servers at URL.
   - Each tweet's retweet count and favorite ("like") count at minimum, and any additional data. Using the tweet IDs in the WeRateDogs Twitter archive, query the Twitter API for each tweet's JSON data using Python's Tweepy library and store each tweet's entire set of JSON data in a file called tweet_json.txt file. Each tweet's JSON data should be written to its own line. Then read this .txt file line by line into a pandas DataFrame with (at minimum) tweet ID, retweet count, and favorite count. Note: do not include your Twitter API keys, secrets, and tokens in your project submission
2. Assess (visually and programmatic): Check gathered data for quality and  tidiness issues.
   - Qualitiy beeing: Completeness, Validity, Accuracy, Consistency
   - Tidiniss beeing: each variable is a column, each observation is a row, each type of observational unit is a table.
3. Clean
   - Requirements for Clean data:
     - Quality requirements:
       - Completeness: All necessary records in dataframes, no specific rows, columns or cells missing.
       - Validity: No records available, that do not conform schema.
       - Accuracy: No wrong data, that is valid.
       - Consistency: No data, that is valid and accurate, but referred to in multiple correct ways.
      - Tidiniss requirements (as defined by Hadley Wickham):
        - each variable is a column
        - each observation is a row
        - each type of observational unit is a table.
4. Analysis & Visualization
5. Store

## Dependencies
The following python libraries are used in the project:
- pandas
- NumPy
- requests
- tweepy
- json

## Known Bugs
