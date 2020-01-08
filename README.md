# Edmunds-Text-Analytics
 This project is a part of the coursework for Text Analytics. Here we scrapped Edmunds.com and implemented various text mining concepts to understand the consumer opinion on car brands and derive insights.

## Team Members:
1. Anshika Ahuja
2. Mohini Agrawal
3. Sachin Balakrishna
4. Pooja Dawada

## Table of contents
- [Introduction](https://github.com/anshikaahuja/Edmunds-Text-Analytics/blob/master/README.md#introduction)
- [Data Used](https://github.com/anshikaahuja/Edmunds-Text-Analytics/blob/master/README.md#data-used)
- [Approach](https://github.com/anshikaahuja/Edmunds-Text-Analytics/blob/master/README.md#approach)
- [Analysis and Insights](https://github.com/anshikaahuja/Edmunds-Text-Analytics/blob/master/README.md#analysis-and-insights)

## Introduction
Edmunds.com is an online resource for automative information. People post reviews about various cars and use the wesbite for awareness building and research. As an analytics consultant to a (i) brand manager, (ii) product manager and (iii) advertising manager, our job was to give advice/insights to these individuals based on the analysis of social media conversations on the website

## Data Used
We scraped around 4000-5000 posts about midsize sedans from [Edmunds](https://forums.edmunds.com/discussion/7526/general/x/midsize-sedans-2-0/p%22) using Selenium. The scraped data can be found in `data.csv`

## Approach
In this project the following steps were taken:
1. Write a scraper using Selenium on python to fetch posts from Edmunds.com
2. Identify the top 10 brands being discussed using frequency counts. Here we replaced car model names with their brand names using the mapping file `models.csv`.
3. Calculate lift scores between brands to identify association between the brands . Plot a multi-dimensional scaling (MDS) map to visualize these relationships.
4. Offer some insights to brand managers for brands identified in the above step.
5. Identify the top 5 most frequently mentioned attributes which people associate with the top brands.
6. Provide suggestions to brand managers of the identified brands based on the above step.
7. Identify the most aspirational brand which people actually want to buy or own from the discussions in the post. What are the business implications of this brand.

## Analysis and Insights

