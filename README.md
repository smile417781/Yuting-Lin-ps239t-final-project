# Yuting-Lin-ps239t-final-project
## Short Description
To see how people talked about some psychological strong indicators of human well-beings(i.e., meaningful life and mindfulness) on Twitter. I majorly used differnet libraries includes rtweet(for collecting data from twitter)/tidyverse&tidytext&tidyr(for tidying data)/igraph&ggraph&ggthemes(for visualizing data). Performing Text mining, Word netword analysis and Sentiment analysis in R. 

First, applied Twitter API randomly retrieving 5000 tweets for meaningful life and 5000 tweets for mindfulness. Second, cleaned data like saving useful text words,removing punctuation, converting to lowercase, adding id for each tweet, storing the token words from each tweet and removing stop words from each tweet for text analysis. Third, made some cute counting word plots by setting them into pinky colors and removing the background, enlarging the font size. Fourth, produced some word network plot by selecting Fruchterman-Reingold layout(one kind of algorithms) for the reason I feel it can presents the data best. Finally, categorized words from tweets by using Bing lexicon to make the data attached with sentiment score and see their pattern in either positive/negative.

## Dependencies

R, version 3.5.1

## Files

### Data

1. meaningful_tweets.csv: row 5000 tweets$text includes "meaningful life" 
2. meaningful_tweets_clean.csv: cleaned version of meaningful_tweets.csv for visualization.
3. mindfulness_pure_tweets.csv: row 5000 tweets$text includes "mindfulness"
4. mindfulness_pure_tweets_clean.csv: cleaned version of mindfulness_pure_tweets.csv for visualization.


### Code

1. 01_collect_twitter.R: Collects data from Twitter API.
2. 02_merge-data.R: Loads, cleans, and merges the raw tweets into useful data.
2. 03_analysis.R: Conducts Text mining, Word netword analysis and Sentiment analysis.

### Results

1. after_meaningful.jpg: after removing the stop words for the tweets includes "meaningful life".
2. after_mindfulness_pure.jpg: after removing the stop words for the tweets includes "mindfulness".
3. before_meaningful.jpg: before removing the stop words for the tweets includes "meaningful life".
4. before_mindfulness_pure.jpg: before removing the stop words for the tweets includes "mindfulness".
5. sentiment_meaningful.jpg: categorized sentiment ranking of tweets includes "meaningful life".
6. sentiment_mindfulness_pure.jpg: categorized sentiment ranking of tweets includes "mindfulness".
7. word network_meaningful.jpg: show the different clusters in tweets includes "meaningful life".
8. word network_mindfulness_pure.jpg: show the different clusters in tweets includes "mindfulness".

## More Information

1.Since all of my codes were written in the same script file and I divided them into three files for the project, somehow the codes runs weird, but all codes worked well together before I did this.

2.After I tried many times of the Twitter API, I found those tweets I got are based on the timeline which is the most recent data. That means if I run the code to retrieve tweets again, it would have different result depend on what people are talking about on twitter right now.

3.Twitter API have the limit for us to get data in a specific time. If you exceeded the number of tweets you can download, it will shows the error like "Rate limit exceeded". But don't worry about this too much, just try it again in like fifteen minutes.
