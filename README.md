# Data-Science-Challenge
The Dataset:
The dataset has (509236, 8) rows and columns respectively.

![Picture1](https://user-images.githubusercontent.com/13540908/76710198-b257ab80-66c2-11ea-8592-db64692fbd6d.png)

The dataset has no missing values. 
The columns "down_votes"  and "category" doesn’t have any unique values. “down_votes” have all the values as 0 and “category” is just ‘worldnews’. As they wouldn’t help in any computation, I have drop them.

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
