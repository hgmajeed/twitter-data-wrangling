# WeRateDogs Data Wrangling
This project is also part of Udacity graduation requirements where focus was on the data wrangling process: gathering, assessing, and cleaning with some minor analyzing and visualizing.

The dataset is the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. Therefore, the rating is not real as you will see that the numerator is always greater than 10, and the denominator is usually equals to 10.  WeRateDogs has over 4 million followers.

### Python Version
- Python 3.7.3

### Required Libraries
- pandas
- numpy
- requests
- json
- tweepy
- timeit
- operator
- matplotlib
- seaborn

### Datasets
The data were obtained from three different sources as follows:
- `twitter-archive-enhanced.csv` was provided by the instructor.

- `image-prediction.tsv` is a file saved at Udacity’s servers where I downloaded it programmatically using requests library. The link is provided in the jupyter notebook file, `wrangle_act.ipynb`.

- For the third dataset, I had to acquire it through twitter API, tweepy, where I established a user application with twitter and created an API object. Then I queried the JSON data from the twitter’s API by supplying the tweet_id columns that I got from `twitter-archive-enhanced.csv`, saved the output to a text file `tweet_json.txt` which I provided in this repository. To reproduce this project, you can either provide your own twitter credentials to recreate the text file, or use `tweet_json.txt` directly. However, you may need to delete the code responsible of creating the files to prevent any error during code execution. 

### Other Files Provided
- `twitter-archive-master`: After cleaning the data, it was saved to this file.
- `wranlge-report.html`: This html file, summarize the data wrangling effort spent on this project.
- `act_report.pdf`: This file summarizes the exploratory data analysis I made on the clean data.
