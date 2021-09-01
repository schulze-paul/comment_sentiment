# A binary sentiment classification Task

The goal of this project is to predict the sentiment of a youtube comment as either positive or negative using supervised machine learning.
The available database consists of two main sources.


## Data

### IMDB movie review dataset

The IMDB movie review dataset consists of 50k datapoints of a review with a binary sentiment rating of positive or negative.

### YouTube dataset

The Youtube comment dataset is a dataset which i manually created where youtube comments are rated with a positve or negative sentiment.

### Train, Train-Dev, Validation and Validation split

| Dataset | Train | Train-Dev | Validation | Testing |
| ------- | ----- | --------- | ---------- | ------- |
| IMDB | 90 | 10 | 0 | 0 |
| Youtube | 72 | 8 | 10 | 10 |

We use a mix of the IMDB and youtube data for training the algorithm.
The Train-Dev dataset is from the same distribution as the train dataset and is used to check if the algorithm can generalize to unseen data from the same distribution as the training distribution.
The validation set and test set are from the target distribution and decide the performance rating of the algorithm

The IMBD dataset as well as the portion of the YouTube dataset are shuffled between the train, train-dev and validation set.
The test set is static and not touched until the end

## Algorithm Architecture

I use an algorithm architecture that has proven to perform well on the IMBD dataset
