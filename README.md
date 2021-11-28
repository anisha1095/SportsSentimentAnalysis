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

## Further Research
