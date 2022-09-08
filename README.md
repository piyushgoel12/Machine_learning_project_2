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
Here I did some data alteration, there are total of 12 columns but for sentiment analysis we only need important features so I've dropped all the unnecessary features for the easy computation of the dataset. So, after the dropping of the data we're left only with the
