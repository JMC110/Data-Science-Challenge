# Data-Science-Challenge
The Dataset:
The dataset has (509236, 8) rows and columns respectively.

![Picture1](https://user-images.githubusercontent.com/13540908/76710198-b257ab80-66c2-11ea-8592-db64692fbd6d.png)

The dataset has no missing values. 
The columns "down_votes"  and "category" doesn’t have any unique values. “down_votes” have all the values as 0 and “category” is just ‘worldnews’. As they wouldn’t help in any computation, I have drop them.


Problem Statement: Categorize News by its Title
After looking at the dataset, the news primarily self-explains itself as political news. As the content of the news articles are not given, I have attempted a topic categorization of news titles from its keywords using Latent Dirichlet Allocation (LDA).
This is an important application of NLP which can help categorize/ Label certain examples of large text. 
