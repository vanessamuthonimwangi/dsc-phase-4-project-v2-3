# Sentiment Analysis of Twitter Feedback Data on Apple and Google Products

## Introduction

According to a [Marquees Brownlee](https://www.youtube.com/watch?v=OFvXuyITwBI&ab_channel=MarquesBrownlee), apple have the best smartphones and products in the world. Is he right? Let's look at the stats. More than 100 million people use Macs globally. Apple had the best-selling smartphones worldwide in 2021. In 2022, iPhone sales were $42.626 billion, versus $38.868 billion the previous year. Revenue for the second quarter of 2023 came in at $94.8B versus the consensus estimate of $92.9B and according to [investing.com](https://www.investing.com/academy/statistics/apple-facts/#:~:text=Apple%20had%20the%20best%2Dselling,million%20people%20use%20Macs%20globally.) as of July this year, apple leads the pack with smartphone market share of 28.39%. Okay so maybe Marquees Brownlee has a point. As the best technology reviewer,Marquees, has over 17 million youtube subscribers with great viewership. Youtubers like him and others influence the 2.1 billion plus active youtube users to take interest or even buy apple products which in part demonstrates the linkage between apple and google product users.

Handling over 90% of all search queries worldwide, Google is undoubtedly dominating the global search engine market share. As of August 2023, a whopping 91.85% of all search queries conducted across all search engine providers are done through the internet giant. Some google products and the number of users are indicated below:
* Google Search - 3.6 billion+
* Android - 3 billion+
* Chrome - 2.65 billion+
* Gmail - 1.8 billion+
* Google Drive - 1 billion+
* Google Maps - 1 billion+
* Google Play Store - 2.5 billion+
* YouTube - 2.1 billion+
* Google Photos - 1 billion+

With the number of apple and google users growing and the use of new slang and new urban abbreviated words rising for example omfgpm, it is increasingly difficult to keep up with the feedback on twitter. 

We can use machine learning to see whether the emotion of a tweet is positive, negative or neutral. Tweets are different that other text data because they are usually in informal conversational language and they they are short. It is important for apple and google to monitor their twitter feed meticulously so as to observe customer opinion and adjust their policies where necessary. If not, they should outsource analytics services from analytics companies.


### METHODOLOGY
The project will follow a structured methodology encompassing the following steps:
* Data Collection: The data was sourced from [here](https://data.world/crowdflower/brands-and-product-emotions). It contains tweet reviews of apple and google products.
* Data Preprocessing: Clean and preprocess the tweet data by removing URLS and hashtags, irrelevant information like special twitter wordsd e.g TR, and performing tasks such as tokenization, and removing stopwords.
* List of libraries used and why:
    * import re #text data preprocessing
    * import string #collection of string functions
    * import nltk #for NLP tasks
    * import pandas as pd 
    * from textblob import TextBlob #NLP library
    * from collections import Counter #frequency analysis
    * import matplotlib.pyplot as plt #plotting visualization
    * from nltk.corpus import stopwords #list of common stop words in different languages
    * from textblob import TextBlob #NLP library
    * from collections import Counter #frequency analysis
    * from sklearn.feature_extraction.text #provides tools for text data preprocessing
    * import TfidfVectorizer #Converts text data into numerical 
* Model: Train a machine learning model (such as a LSTM, GRU and RNN for deep learning model) using the preprocessed dataset to classify tweets into positive, negative, or neutral sentiments. Evaluate the model's performance using appropriate evaluation metrics. (ADD MORE]
* Evaluation: 


* Insights and Recommendations: Analyze sentiment analysis results to generate actionable insights and recommendations for improving customer satisfaction, addressing pain points, and managing brand reputation effectively.
* Response and Engagement Strategy: Develop a strategy for airlines to respond to negative sentiment and engage with customers in a timely and personalized manner. Implement systems and processes to manage customer feedback, complaints, and turnaround negative experiences into positive ones.

### PROBLEM STATEMENT

The expanding market presence of Apple and Google products has resulted in a significant surge in their user base within the industry. This expansion has, in turn, generated a substantial volume of feedback from customers expressing both satisfaction and dissatisfaction, with a notable portion of this feedback originating from Twitter. Consequently, addressing these customer concerns and proactively improving the overall perception of their respective brands has become a paramount priority for both Apple Inc. and Google.

####  SPECIFIC OBJECTIVES

1. To develop a real-time monitoring system capable of retrieving and classifying live tweets related to Apple and Google products using the sentiment analysis model, ensuring scalability to handle high volumes of incoming tweets.

2. To conduct an in-depth analysis of the sentiment classification model's performance and fine-tune it for optimal accuracy and efficiency.

3. To explore the feasibility of integrating additional sources of customer feedback, such as customer reviews on e-commerce platforms, into the sentiment analysis system to provide a comprehensive view of customer sentiment beyond Twitter data.


## DATA UNDERSTANDING

The data was sourced from [here](https://data.world/crowdflower/brands-and-product-emotions).

## FINAL MODEL

My final and preferred model is the untuned LSTM which performed better compared to other models with an accuracy of 96 percent. 


## CONCLUSIONS

- Sentiments expressed by customers play a significant role in their decision to continue or discontinue their relationship with a product therefore negative sentiments should be addressed.
- The model has proven to have an accuracy of 96% in classying whether a tweet is postive, negative or neutral and it can be used to continuosly monitor the sentiments coming from the social media platforms.

## **MODEL LIMITATIONS**

- The model struggled to classify positive sentiment tweets, especially in the LSTM and GRU models.
- Identofying slang words and urban abbreviations to include in sentiment analysis. Since twitter will be heavily used by the Gen Z and Gen Aplha users, we need to create sentiment analysis that incorporates informal language that they use.

## **RECOMMENDATIONS**

Future steps: Integrate additional sources of customer feedback
•	While this objective is not explicitly addressed in my project, there's a possibility of extending the sentiment analysis system to include other sources of customer feedback, such as e-commerce reviews. This can be done as part of future work or enhancements to the project.
•	There is an emphasis on real-time monitoring and scalability sets the stage for incorporating additional data sources seamlessly in the industry.
