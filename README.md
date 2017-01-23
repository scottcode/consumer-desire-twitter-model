# consumer-desire-twitter-model
Code for building a binary classification model in Python to classify Tweets as either related to individual consumer desire or not. 

## Contents
* Jupyter notebooks
  * 01_parse_tweets.ipynb
  * 02_model_intent.ipynb: build and pickle classification model
* labels_tesla.txt: key of labels used in '...labeled.csv' below
* tesla_tweets_rand_for_label_2017-1-6_labeled.csv: labled tweets
* raw tweets in JSON line format
  * teslatweet_2017-1-5.gz
  * teslatweet_2017-1-6.gz
* Pickled models
  * twitter-consumer-desire-logreg.pkl
  * twitter-consumer-desire-pipe.pkl: use this one; it includes feature generation


## Label Definitions

Symbols used in the label column (in `label: definition` format)

* `0`: can't judge (in another language, only a link, etc) 
* `n`: not about tesla company/product 
* `m`: only about Musk himself 
* `v`: about business, news, current events 
* `i`: by an individual 
* `c`: by a company 
* `d`: individual consumer desire/opinion 
* `b`: intent to buy 
* `+ -`: positive or negative sentiment 
