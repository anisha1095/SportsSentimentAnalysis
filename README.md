# Sports Sentiment Analysis

This project aims to find the sentiment trends across matches from influential twitter fan accounts as well as official team and player accounts. We hypothesize that the Public Relations Teams of the official accounts keep posting positive tweets even when having bad results to maintain a positive image of the club but the fan accounts reflect the actual sentiments about the results of the football club. 
For our analysis we are analysing fan tweets of Manchester United Football Team. 

## Table of Contents
1. Dataset
2. Methods Used
3. Analysis
4. Further Research

## Dataset 
Tweets are extracted from Tweepy API of Twitter for the following accounts on specific match dates. 

## Methods Used

Sentiment Analysis using Vader. (https://github.com/cjhutto/vaderSentiment#python-demo-and-code-examples) 
Vader Library provides 4 scores - neu, pos, neg and compound. 

The compound score is computed by summing the valence scores of each word in the lexicon, adjusted according to the rules, and then normalized to be between -1 (most extreme negative) and +1 (most extreme positive). This is the most useful metric if you want a single unidimensional measure of sentiment for a given sentence. Calling it a 'normalized, weighted composite score' is accurate. - 

The sentiment is calculated on compound score - 
Positive : compound score >= 0.05
Neutral : (compound score > -0.05) and (compound score < 0.05)
Negative : compound score <= -0.05

## Analysis 
Fan Sentiments Trends -- 

<img width="468" alt="Screenshot 2021-12-05 at 12 21 02 AM" src="https://user-images.githubusercontent.com/10363259/144736106-a8b0bd8a-15f0-4394-99fd-2cab56a6a036.png">

Official Accounts Sentiment Trends --


<img width="417" alt="Screenshot 2021-12-05 at 12 27 30 AM" src="https://user-images.githubusercontent.com/10363259/144736241-b71569a9-24b3-4ad8-be76-892a612f82ec.png">

## Further Research
