#### **Demystifying Optimization bias**

I was working on a side project with my friends recently, whereby we were attempting to carry out sentiment analysis on the IMDB dataset. The dataset was curated by Andrew Maas, and it contains 50,000 movie reviews (it can be found [here](https://www.kaggle.com/utathya/imdb-review-dataset/download)). After training our model using a training set of 500 observations (out of 50000), we evaluated the model by optimising the **max_df** hyperparameter (which is used to detect and filter stop words) of [CountVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.CountVectorizer.html), and **regularization** (C) hyperparameter of the [LinearRegression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html) model and exhaustively searching for the best hyperparameters through cross-validation. The results are displayed in the table below: 



