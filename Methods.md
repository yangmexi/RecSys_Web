---
title: Methods
notebook: Methods.ipynb
nav_include: 2
---

## Contents
{:.no_toc}
*  
{: toc}

## Train and Validation Set



## Metrics

## Modeling Approach

### Baseline Model

To compare the performance of 

### Collaboratvie Filtering

Collaborative filtering is a common technique for recommendation systems. It is based on the assumption that people will like items that are similar to other items they like, and people will like items that are liked by other similar people. There are two types of collaborative filtering models, which are memory-based and model-based collaborative filtering. Memory-based approaches establish similarity matrix between either items or users, whereas model-based approaches further fill out the matrix with several machine learning algorithms to predict how likely a new item will be picked by a user.

#### Memory-based Approach

##### Item-based

We created a cosine similarity matrix between each playlist in train dataset. When we did recommendations for a specific playlist, we looked at each new song that was not currently in this playlist and all other playlists including that new song. We added the user-to-user similarities for those playlists to generate a new similarity score and ranked all new songs by this new similarity. Then we recommended 500 songs for each playlist based on this new similarity score. Instead of simply equally recommending all songs from a similar user, this approach enabled us to generate rank for each new song recommended.

##### User-based

For our item-to-item model, we first created a cosine similarity matrix between each item (song) in the train dataset (of the 1000-playlists subset). This resulted in a similarity matrix of size 32643 * 32643. Using the similarity matrix, the top 700 neighbors (top 700 most similar songs) of each song were found and put into a Pandas DataFrame of size 32643 * 700. Next, for each input song, we retrieved its neighbors and compiled them together into a 1-d numpy array. After removing all repetitive songs and songs that are in the input playlist, we recommended the songs with the top 500 similarity scores. 

#### Model-based Approach

##### KNN

##### ALS

##### NN
