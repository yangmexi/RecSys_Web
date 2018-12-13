---
title: Final Report - Automatic Playlist Recommender
---

**Group 45 🎧: Lucy Liu🎹, Mengxi Yang👾, Rui Song🌦, Tong Zhao🎀**

## Overview

As of date, according to data released by Apple’s app store and Google Play, Spotify is the most popular music application in the United States. Spotify’s success consists of many facets, and its well-performing music recommender system undoubtedly plays an integral part. In all, Music recommender systems (MRS) have recently exploded in popularity thanks to popular music streaming services like Spotify, Apple music, etc. By some accounts, almost half of all current music consumption is by the way of these services. The popularity of music recommender systems is intelligible. Through technological advances, the mainstream way of music consumption evolved from using individual devices CD players, walkmans, iPods as ‘music players’ to using apps on laptops and mobile phones. A main change associated with the change of mainstream devices is that, a user’s ‘playlist’ is no longer ‘locally stored’, but rather stored online and can be shared with other users online. Public playlists on Spotify can be ‘followed’ by other users, and updates on the playlist are immediately available to followers.  As a result, online playlists possess properties that allow them to be dynamic and timely, and would therefore attract more user usage and interactions.

Automatic playlist generation is about finding the set of songs to recommend to best extend the experience of a listener in the midst of a playlist. By suggesting appropriate songs to add to a playlist, a Recommender System can increase user engagement by making playlist creation easier, as well as extending listening beyond the end of existing playlists.

![Image result for spotify logo](https://developer.spotify.com/assets/branding-guidelines/logo@2x.png)

## Project Goal

Our goal is to build a well-performing Music Recommender System that recommends songs to add into existing playlists. We decided to tackle the problem with several models. Each model will recommend 500 songs for each query playlist and their performances will be evaluated and compared. 

## Challenge

During the execution of the project, a major challenge was the size of the MPD. It is beyond our computers’ capacity to work with such a huge dataset locally. We therefore decided to use only a subsample of the data, working with 1000 playlists randomly selected from the MPD. More on this is described below. 
