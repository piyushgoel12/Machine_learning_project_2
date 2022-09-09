Introduction
---------------
This is another machine learning project by me, here I took Amazon reviews on several products and performed sntiment analysis on the same to witness results that may help the repsected comapny to help or satisfy the unsatisfied customers or improve their services for a better UI/UX experience. 

Dataset
---------------
The dataset that I'll be using is "Amazon reviews for sentiment analysis", I've dowloaded this dataset from Kaggle. The link for the same is: https://www.kaggle.com/datasets/tarkkaanko/amazon

The dataset contains 4914 rows and 12 columns, there are several features in the dataset but only a few of them are important for us to perform sentiment analysis. The important columns or features are explained below: 
1. Reviewer Name: The username of the user who has posted the review. (It's important just for the verification if a particular user posted a given review or not.)
2. Overall: This column represents the ratings given by the users(The maximum being 5.0 and the minimum being 1.0). 
3. reviewText: This column represents the textual data or the review posted by the user for their product. 

Data Modification 
----------------
Here I did some data alteration, there are total of 12 columns but for sentiment analysis we only need important features so I've dropped all the unnecessary features for the easy computation of the dataset. So, after the dropping of the data we're left only with the three features that are important for the sentiment analysis of the dataset. The features that we are left with are: 
1. Reviewer Name: The username of the user who posted the review of their specific product. 
2. Overall: This represents the ratings that the user posted. 
3. reviewText: This is the actual review that the user posted and it's an important aspect for the sentiment analysis. 

Data pre-processing
-----------------
Now that we have dropped all the unimportant columns or the features it's time to process the data. And the first step is to check if there's any missing/null values in our dataset and there appears to be some missing values but the number of missing values in the dataset are far way lesser than the total number of instances so we can just drop those rows with the missing values with the help of 'dropna()' function. 

After removing the null values from the dataser it's time to clean the data and remove unwanted puntuations and I've done it using NLP(Natural Language Processing). 

Data Visualization
-------------------
I've cleaned the data and also processed it using NLP, now is the time to visualize the data and draw important outcomes from the same.
Firstly I've visualized the 'Overall' (Ratings) column using a pie chart and here we can see that maximum number of reviews (79.8%) posted have 5 star ratings. So, we can easily say that many users are satisfied with their products while only 4.9% of the total users have provided 1 star rating. 

Now I've tried to visualize the type of review user have left on the webiste using the wordcloud. 

The wordcloud results can be seen and essential information can be drawn fromn them. 

Now I added some more columns in the dataset for sentiment analysis, the new columns being 'Postive', 'Negative', and 'Neutral' for presenting the sentiment scores of the Amazon reviews. 

After adding the new columns I checked the response that has the highest score among the all three. 
Most of the users have 'Neutral' response towards their product ordered from Amazon. 

Now finally, let's see the total sentiment scores of the all three columns namely, 'Positive', 'Negative', and, 'Neutral'. 
So, we can see that most of the users have neutral feedback for the services provided by Amazon while a small amount of users had Negative response.

Conclusion
--------------
So, here we can see that most of the users are neutrally satisfied with the services provided to them while a small amount of users have Negative feedback towards them, hence this sentiment analysis of the Amazon reviews helped us to view the sentiment of users towards Amazon. Further more upgradations can be done on this code such as introducing LSTM or several Deep learning models for better sentiment analysis of diferent type of data. So, that was all for this project. 

You may contact me via Linkedin: https://www.linkedin.com/in/piyush-goel-6974b4203/
