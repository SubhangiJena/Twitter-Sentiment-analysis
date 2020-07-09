# Twitter-Sentiment-analysis
Sentiment Analysis model to categorize a tweet as Positive or Negative 

Sentiment Analysis: It is the interpretation and classification of emotions (positive, negative and neutral) within text data using text analysis techniques. Sentiment analysis allows organizations to identify public sentiment towards certain words or topics.


MODEL PIPLINE


    Importing dependencies
    Importing dataset
    Preprocessing Text
    Analysing data
    Splitting data
    TF-IDF Vectoriser
    Transforming Dataset
    Creating and Evaluating Models
        LinearSVC Model
        Logistic Regression Model
  
  
  
Importing dataset

The dataset being used is the sentiment140 dataset. It contains 1,600,000 tweets extracted using the Twitter API. The tweets have been annotated (0 = Negative, 4 = Positive) and they can be used to detect sentiment.


t contains the following 6 fields:

    sentiment: the polarity of the tweet (0 = negative, 4 = positive)
    ids: The id of the tweet (2087)
    date: the date of the tweet (Sat May 16 23:58:44 UTC 2009)
    flag: The query (lyx). If there is no query, then this value is NO_QUERY.
    user: the user that tweeted (robotickilldozr)
    text: the text of the tweet (Lyx is cool)
    
    
    Only using sentiment and text fields, so discard the rest.
    
    Furthermore, we're changing the sentiment field so that it has new values to reflect the sentiment. (0 = Negative, 1 = Positive)
    
      Preprocessing Text:
            Lower Casing
            Replacing URLs
            Replacing Emojis
            Replacing Usernames
            Removing Non-Alphabets
            Removing Consecutive letters
            Removing Short Words
            Removing Stopwords
            Lemmatizing
    
    Analysed data using word cloud
    split the data into training and test data
    
    Transforming the X_train and X_test dataset into matrix of TF-IDF Features by using the TF-IDF Vectoriser.
    This datasets is used to train the model and test against it.
    
    Implementing using two models
        Linear Support Vector Classification (LinearSVC)
        Logistic Regression (LR)
        
    Predictions:
    I am  choosing Accuracy as evaluation metric.
    Also ,plotting the Confusion Matrix to get an understanding of how  model is performing on both classification types.
    
    Logistic Regression Model nearly achieves 82% accuracy while classifying the sentiment of a tweet.
    LinearSVC Model performswith  81% accuracy while classifying the sentiment of a tweet.


