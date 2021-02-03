# Top-5-Articles-with-relevant-Keywords-extraction-
This task aims to fetch Top 5 articles from internet and show related keywords, titles with it.



Queries answered:

1. Approach to the solution:
ANSWER: Used Tfidf Vectorizer to seek most relevant words from article, getting information from link using regex, query suggestion were extracted from wikipedia and some other resources. Also took advantage of tfidf vectorizer and simply regex to fetch top 5 articles.


• Which ML/DL model architecture you used and why?
ANSWER: Due to insufficency of data, haven't used any ML/DL algorithm, but did create intelligent program that does pattern matching within the fetched articles and seek for best 5.

• How would you ensure the scalability of your solution?
ANSWER: The code is suitable for any sort of queries, except news articles.

• Is there a need for any dataset? If yes then how much data is
sufficient to train the model in order to get required results?
ANSWER: The approach I have used does not required any dataset, but to use fetched one itself. But for categorization part, there is need of dataset as many possible categories. 
It also depends on whether we need to have a definite set of categories or not. 


• Is there a need to create manual datasets, if yes then what
parameters and sample size did you consider to create a dataset?
ANSWER: For temporarily for this approach. But if we use different algorithm, say GPT-1,2,3 or BERT, we might need to create manual dataset for categories, corpus of all previous searches, 

• Are your model and dataset generalized enough for different
domains of the use cases, How?
ANSWERS: While performing vectorization part, I had an observation, that words with frequency are more related to different domains, Thus, the searched articles might not focused to specific domain. Categorization part is still on work.


• How would you train, test and deploy your model to production?
ANSWER: No train test has been done in this approach.

How would you perform hyperparameter tuning on your model to
improve accuracy?
ANSWER: To get better results, I have used GridSearchSV for tfidf Vectorizer part.

• Anything else you want to let us know about your approach.
ANSWER: The approach is just a base model. The model needs to get more additions onto adding up categories and this can be possible by fetching categories from all relevant sources like wikipedia, geeksforgeeks, etc using wikiextractor.


3. Only Approach to generate different types of questions (short
answer type, MCQs, true/false, fill in the blanks, long answer type
etc.) for that same article.
ANSWER: We can use R-Net model for this approach. The choice was made in favor of this model because of its good score on state-of-the-art leader boards and a well-described architecture. The R-Net model is based on Bidirectional Recurrent Network where question and passage are processed separately. 
