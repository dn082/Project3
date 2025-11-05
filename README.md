# Project3

## INTRODUCTION
In this project, I chose to analyze a data set that has information on over 30000 Spotify Songs that came from the Spotify API, and will predict a song's popularity score. This can solve the general idea of the concept of predicting the success of a song based on features it can have, such as danceability, energy, loudness, acousticness, tempo, and many other features. 

## THE DATASET
The data I chose to use is a file found from Kaggle called https://www.kaggle.com/datasets/joebeachcapital/30000-spotify-songs/data. My target variable is track_popularity, and I will be using attributes of an audio to predict the song's popularity.

## WHAT IS REGRESSION AND HOW DOES IT WORK?
Linear regression is the concept of supervised learning being used for prediction, and a statistical and machine learning method used to model the relationship between a dependent variable and one or more independent variables by fitting a straight line like a linear line.

A formula to represent the basic idea is
y = beta0 + beta1 * x + epsilon

y = the variable you are trying to predict - dependent
beta0 = the value of y when x = 0
beta1 = 
x = the input - independent
epsilon = error term

## PREPROCESSING
Some steps I took for preprocessing my data were to:
  -  Checking for Missing Values and Dropping Irrelevant Columns  - Doing this step allowed me to simplify my data and be able to encode, as I dropped all rows that contained any missing   values, along with dropping several columns that were irrelevant for the analysis or could lead to issues with encoding or regression.
  - Used One Hot Encoding - Doing this step allowed all the columns to turn text categories into numbers that the Linear Regression model can use and understand, which is usually binary.

## MODELING/ EVALUATION
- Experiment 1 - My first experiment using Linear Regression to predict song popularity based on 489 features, including audio characteristics and the encoded genre/playlist categories. I got decent results coming from that many features
- Experiment 2 - For my second experiment, I wanted to use the same thing, so I decreased features as I removed the playlist_name column before encoding and training the model. By removing it, the R2 reduced, and it increased the RMSE, meaning it is not ideal as the concept for its popularity was better off in the last one, but with fewer features, it makes the model less complex.
- Experiment 3 - For my third experiment, I essentially used the same features as experiment one, but changed to model, and it got the same results I thought it would change, as it was ideal for dealing with larger data.

## IMPACT
I think it can be impactful in the way that the popularity and trends could be based on other attributes that are not by genre or artist, but instead focus on different traits, which can help create an unbiased recommendation system and create trends that are based on sound that are ideal for that season, such as low-tempo music, and etc.

## CONCLUSION
Through this project, I learned;
- To apply pre-processing and encoding.
- Be able to apply Linear and Ridge models.

## REFERENCES
- https://www.kaggle.com/datasets/joebeachcapital/30000-spotify-songs/data
- https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Ridge.html 
