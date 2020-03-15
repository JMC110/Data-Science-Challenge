# Data-Science-Challenge
**The Dataset:**
The dataset has (509236, 8) rows and columns respectively.

![Picture1](https://user-images.githubusercontent.com/13540908/76710198-b257ab80-66c2-11ea-8592-db64692fbd6d.png)

The dataset has no missing values. 
The columns "down_votes"  and "category" doesn’t have any unique values. “down_votes” have all the values as 0 and “category” is just ‘worldnews’. As they wouldn’t help in any computation, I have drop them.

**Word Cloud of all the News Titles-**

![wordcloud](https://user-images.githubusercontent.com/13540908/76710234-0793bd00-66c3-11ea-8f7a-886b44f4619c.png)


**Problem Statement: Categorize News by its Title**

After looking at the dataset, the news primarily self-explains itself as political news. As the content of the news articles are not given, I have attempted a topic categorization of news titles from its keywords using Latent Dirichlet Allocation (LDA).
This is an important application of NLP which can help categorize/ Label certain examples of large text. 

**Solution:**
 
**Steps performed in this challenge:**

1) EDA with word clouds
2) Preprocessing of News “Titles”
3) Afinn Sentiment Analysis
4) K Means Clustering
5) PCA
6) Latent Dirichlet Allocation (LDA) for automatic labeling and categorization of news by its “title”
7) pyLDAvis chart to visualize the produced labels and its associated keywords

**The LDA Model-**
The “titles” are tokenized into a list of words and a Bigram and Trigram of the words is generated. 


**Bigrams**- two words occurring frequently in a document.

**Trigrams**- Three words occurring frequently in a document.

The input to the LDA model is a dictionary and the titles. Genism creates a unique ID for each of the word in the titles document. LDA model is easy to build with Genism. LDA model gives a Label suggestion and gives the following output with scores of each keyword contributing to that Label

![image](https://user-images.githubusercontent.com/13540908/76710303-a8827800-66c3-11ea-9285-ea8a71aabdf6.png)


**The Afinn Score:**

The dataset is self-explanatory and could be used for a better sentiment analysis if the feature “down_votes” had better understanding. Here I have used the “afinn-score” which provides a word-list based approach. Following is an easy example to understand afinn score-

![Snip20200315_4](https://user-images.githubusercontent.com/13540908/76710233-0793bd00-66c3-11ea-9e82-cbd46183bdf9.png)

**Afinn Score for the News Titles:**

![Snip20200315_2](https://user-images.githubusercontent.com/13540908/76710231-05c9f980-66c3-11ea-8dba-fc0ffdc72b2b.png)


**Conclusion:** 
Perplexity and Topic Coherence are measures to evaluate how good the topic modeling is. Perplexity is better when its lower.
Whereas Coherence measure is evaluated by measuring the degree of semantic similarity between high scoring words in a topic. It basically helps distinguish between good and bad topics. 

pyLDAvis represents all the topics/labels selected and the words associated to it.
The Perplexity and Coherence score for the year 2008 news Titles-

![image](https://user-images.githubusercontent.com/13540908/76710419-a79e1600-66c4-11ea-9bf8-10bdb770ac67.png)

*Kindly use NBviewer for visualizing the pyLDAvis.*
