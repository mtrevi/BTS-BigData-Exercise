# Data Analysis Exercices

## Get Pandas

For Mac OSX / Linux / Windows:

- [Anaconda](https://www.continuum.io/downloads) (collection of python libraries) – recommended with Python 3.5

Additional Software for Mac OSX:

- [Pineapple](https://nwhitehead.github.io/pineapple/) – recommended with Python 3.5

Do it by yourself:

- Install `Python 3+` and `iPython 3+`, then with `pip` install all the dependences (jupyter, numpy, scipy, pandas, etc.) and run your notebook by your *shell*.


## Some References

Cheatsheets for Data Analysis in Pandas

- [11 steps for DS in Pandas](http://www.analyticsvidhya.com/blog/2015/07/11-steps-perform-data-analysis-pandas-python/) by AnalyticsVidhya
- [short commands description for Pandas, SciPy, NumPy and Quandl](https://s3.amazonaws.com/quandl-static-content/Documents/Quandl+-+Pandas,+SciPy,+NumPy+Cheat+Sheet.pdf) by Amazon

Visualization with `ggplot`:

- [*ggplot* introduction](http://ggplot.yhathq.com/) by Yhat
- [*ggplot* graphic explained](http://r4stats.com/examples/graphics-ggplot2/) by r4stats
- [using *ggplot* in Python and R](http://blog.yhat.com/posts/ggplot-for-python.html) by Yhat

Need to play with some fancy dataset? Then check out the [Kaggle Datasets](http://blog.kaggle.com/2016/01/19/introducing-kaggle-datasets/) by Ben Hamner released on the 19-01-2016.

## Exercise: Pandas *vs* SQL

Again the same questions but this time find their answers with `pandas`.

Few quick notes just to start:

```python
# import some useful libraries
import pandas as pd
import numpy as np

# load the tsv file into a dataframe
data_path = '<write_here_the_path_of_twitter-vine-clean.tsv.bz2>'
df = pd.read_csv(data_path, sep='\t', compression='bz2')

# start to play with it
df.head()
```

### List of Questions

1. How many tweets?
2. How many unique users?
3. How many tweets contains more than one URL?
4. How many tweets are geotagged (have `latitude` and `longitude`)?
4. How many tweets are original (*e.g.*, not retweets)?
5. How many tweets for each day? In average?
6. Day of the week with highest volume of traffic?
7. Which are the most popular `user_location`?
8. Which are the most popular hashtags?

#### Advance Questions

1. Can you create and display a DataFrame with the following columns: 
```
created_at, user_id, no_followers, no_tweets, no_tweets_with_retweets
```
2. Can you plot an histogram with the number of tweets per day? 

### Push the Results in your GitHub

The questions with the results need to be saved in a MarkDown file called `twitter-sql-exploration.md`, inside a `sql-exercise` folder of your github repo.
