# Coronavirus analysis

This repo analyzes the activity of coronavirus hashtags on twitter. We have processed a dataset of all geotagged tweets that were sent in 2020. The size of this dataset is about 1.1 billion tweets. Following the MapReduce procedure, we analyzed these tweets based on what coronavirus related hashtags were used. The hashtags we selected for include: 
- `#코로나바이러스`
- `#コロナウイルス`
- `#冠状病毒`
- `#covid2019`
- `#covid-2019`
- `#covid19`
- `#covid-19`
- `#coronavirus`
- `#corona`
- `#virus`
- `#flu`
- `#sick`
- `#cough`
- `#sneeze`
- `#hospital`
- `#nurse`
- `#doctor`
Starting with JSON files of the tweets partitioned by day, we processed each file to provide a summary of the number of tweets for each hashtag, organized by language and country. Finally, we visualized the combined results to determine the most used languages and countries for each hashtag. These visualizations can be found in the viz folder.
We found that almost all hashtags were used most in English (all except those in characters specific to different languages). For those hashtags in characters specific to different languages, each was used most by that language. For example, the Chinese hashtag (`#冠状病毒`) was used most in Chinese and hardly used in any other languages. 
We also found that a lot of hashtags were used most from the US. Again, for those hashtags in characters specific to different languages, each was used most by that the native country of that language. For example, the Japanese hashtag was used most in Japan. It is interesting to note that both `#covid-19` and `#covid2019` were used most in India and #virus was used most in Britain.
Finally, we found that `#corona`, `#coronavirus`, and `#covid19` were the most used hashtags, while words more generally related to illness (such as `#hospital`, `#nurse`, `#sick`) were used almost ten times less.

