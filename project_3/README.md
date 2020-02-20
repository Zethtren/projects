# Differentiating Subreddit Posts using Natural Language Processing Methods

### The Question:

First we ask if we can differentiate between the posts of two subreddits using machine learning models. In order to explore this question I chose to use the AskScience and AskEngineers Subreddits.

These subreddits seem similar but have different vocabulary used in posts. 

### The Data:

I used PushShift API to collect information from Reddit. I specifically passed filters into the API to only collect posts from non-deleted users and to collect the API suggested maximum of 500 from each subreddit.
[https://pushshift.io/]

After pulling the Data I removed all except for 1 identifying features. I kept information regarding the time of post, the number of followers, the number of crossposts, the body of the text, and post score.

I then combined the data into a single dataframe and ran a train_test_split on it. 

Once the Data was split I vectorized the text using CountVectorizer.

### The Models:

In this workbook I explored 4 different models and received excellent results from all of them. 

##### The Models I explored and their respectives training and testing scores:

|**Model:**| Random Forest | Support Vector Machine | XGBoost Random Forest | XGBoostClassifier |
|----------|---------------|------------------------|-----------------------|-------------------|
| Training | 100%          | 98.2%                  | 98.4%                 | 99.7%             |
| Testing  | 94.8%         | 98.4%                  | 98.4%                 | 99.6%             |

The XGBoost Classifier had near perfect Accuracy. I omited it from my results since I can't explain the math behind how it works. And we haven't discussed it in class.

The Random Forest and Support Vector Machines both scored highly as well. 

This indicates there is some kind of pattern in the data.

### Exploring the Results:

There were 301 words that only appeared in the AskScience Subreddit.
There were 1208 words that only appeared in the AskEngineers Subreddit.


Words that occured only in the Science posts and their respective counts:

| Top 40 words   | Count| 
|:---------------|---:|
| ut             | 53 |
| et             | 52 |
| twitter        | 37 |
| edu            | 36 |
| nih            | 36 |
| cells          | 35 |
| ama            | 29 |
| ph             | 26 |
| ut ask         | 26 |
| nih gov        | 25 |
| your questions | 24 |
| twitter com    | 24 |
| https twitter  | 24 |
| ask us         | 22 |
| us anything    | 21 |
| we ll          | 18 |
| scientists     | 18 |
| institute      | 18 |
| scientific     | 18 |
| me anything    | 17 |
| biological     | 17 |
| published      | 17 |
| answer your    | 16 |
| 16 ut          | 16 |
| neutrons       | 15 |
| 19             | 15 |
| disease        | 14 |
| black          | 14 |
| 00             | 14 |
| species        | 13 |
| mission        | 13 |
| medicine       | 13 |
| the brain      | 13 |
| population     | 13 |
| children       | 13 |
| emotional      | 12 |
| dna            | 12 |
| stars          | 12 |
| et 16          | 12 |
| articles       | 11 |  



Words that only occured in the Ask Engineers Subreddit:

| Top 40 Words           |Count|  
|------------------------|-----|
| mechanical             | 68  |
| advice                 | 57  |
| the company            | 43  |
| internship             | 42  |
| interview              | 40  |
| thank you              | 39  |
| thank                  | 39  |
| guys                   | 36  |
| my first               | 32  |
| to work                | 32  |
| mechanical engineering | 30  |
| any advice             | 30  |
| offer                  | 29  |
| graduated              | 27  |
| am currently           | 27  |
| my career              | 27  |
| to start               | 26  |
| of engineering         | 25  |
| boss                   | 25  |
| positions              | 25  |
| an engineer            | 24  |
| in engineering         | 24  |
| path                   | 23  |
| it was                 | 23  |
| motor                  | 23  |
| you guys               | 23  |
| ee                     | 22  |
| sector                 | 22  |
| asked                  | 21  |
| my resume              | 21  |
| interviews             | 21  |
| civil                  | 21  |
| is my                  | 21  |
| my job                 | 20  |
| if anyone              | 20  |
| pay                    | 20  |
| mostly                 | 20  |
| an engineering         | 20  |
| know if                | 20  |
| salary                 | 19  |


It's probable that these were the main influencers in the models success.
