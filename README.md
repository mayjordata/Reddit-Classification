# Language analysis between users on the r/NFL & r/fantasyfootball subreddits

### Problem Statement

I will use data collected from posts on the NFL and Fantasy football subreddits on the popular website reddit.com to build a logistic regression classification model to predict which subreddit a post belongs too. By analyzing the language used in both subreddits I seek to understand how to improve fan engagement for the NFL.


### How to use this Repo

it’s recommended to use each of the notebooks in sequence of:

- 01_Reddit Scraping
    * For this notebook, you need to create/obtain a Reddit account.
    * visit site & save user account into a json file and save it to the assets directory. This file is your key to begin scrapping data from the site.
- 02_EDA & Language Processing
- 03_Grid search & Modeling

---

### Results
*TFIDF Vectorizer used

Parameters:
- N-grams: 1 to 3 words
- Max features: 100,000
- Max Document Freq: 30%
Logistic Regression Model with Ridge Regularization

Accuracy Score: 94% 


---

### Conclusion & Reccomendations

The Vectorizer that I chose to perform my analysis on along with my model was the TFIDF. This is in part because, due to the high activity on both subreddits, there are several posts that mentions the same word several times in the same post. Though my model suffers some with the TDIDF, it helps in minimizing this issue for analysis purposes. 
The top findings were the sentiment of posts in the r/fantasy football being slightly more positive than the r/NFL posts. Player's names show up a lot more frequently in the posts, meaning that a lot of the focus are on the players and not so much the game.

The NFL should look into integrating this fact into how the game is played and Marketed.


   
