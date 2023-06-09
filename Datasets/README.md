## Datasets

### Blodgett

The authors of the original paper say they used 50,000 tweets from the Blodgett dataset that had a high likelihood (greater than 90%) of AAE dialect as predicted by their model. 

The file "Blodgett_50k_IDs.csv" contains the IDs of 50,000 Tweets that we used in our reproduction, that were still available via the Twitter API at publication time. You can use the Twitter API to retrieve these tweets with the notebook "02_Retrieve_twitter_data.ipynb". However, some of the Tweets may have become unavailable (if they are deleted or removed from Twitter) since publication time.

To create this list of Tweet IDs, we downloaded the file "TwitterAAE-full-v1.zip" from [TwitterAAE: Research on African-American English on Twitter
](http://slanglab.cs.umass.edu/TwitterAAE/). From this dataset, we selected the IDs of Tweets that have a high probability (greater than 90%) of being AAE, according to the Blodgett model - this probability is given in the data files. This left 548,516 Tweets. We used the Twitter API to retrieve the first 50,000 Tweets that are still available.  (Note: the file "TwitterAAE-full-v1.zip" also contains the Tweet text, so it does not strictly need to be re-retrieved from Twitter.)

To train a `word2vec` file, we used the 548,516 Tweets from Blodgett that were classified as having greater than 90% likelihood of being AAE dialect. You can generate the "Blodgett_500k.csv" dataset from the "Blodgett_500k_IDs.csv" file using a similar approach.

### DWMW17

We retrieved the ["labeled_data.csv"](https://github.com/t-davidson/hate-speech-and-offensive-language/blob/master/data/labeled_data.csv) file from [Automated Hate Speech Detection and the Problem of Offensive Language](https://github.com/t-davidson/hate-speech-and-offensive-language) and named it "Dwmw17.csv".

### FDCL18 

We downloaded the FDCL18 dataset from [Intersectional Bias in Hate Speech and Abusive Language Datasets](https://github.com/jaeyk/intersectional-bias-in-ml) and named it`fdcl18.csv`.
