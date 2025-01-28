## Music App Project 

## Genre Music Prediction Using Machine Learning

## Team Members: 
- **Nathaly Lamas**
- **Olga Petrova**
- **Feda Zidan**
- **Harrison Teyfur**
- **Ouyang Beiting**
- **Lakshay Garg**

## What does this project do

## The project uses a trained machine learning model to predict music genres from listening to provided MP3 snippets of music.

## How it works:
**The music App** is connected to the user's [Spotify](https://open.spotify.com/) account. User is offered to search a song of liking, app gets the preview of the song online. This preview song then gets into the preprocess step and gets sliced to 3 second segments. Using **Librosa library** features extracted in the same process. The program checks to see if the song's features are the similar to trained model features. Then the preprocessed song gets through the saved machine learning model and predicts the genre of the preview song.
The matching genre is then sent into in the App for the song recommendation. App pulls 20 new song recommendations with matching genre for User. User can create a new playlist with the recommended songs by swiping right or left.  User can add these songs to their **Spotify** account as a playlist.


## Why it's important
Sometimes we hear a song on Spotify and want to find songs in the same genre. Unfortunately Spotify doesn't explicitly say what is the genre of the song it just played.

We provide this option. Groovr uses machine learning algorithm to define song's genre and helps to find songs from the same genre. This way we can create different playlists to match different moods.


## The choice of machine learning model: 
The machine learning model we used was **CatBoost**.

**CatBoost** (Category Boosting) is a type of machine learning algorithm that uses gradient boosting on decision trees. It’s available as an open source library: [https://catboost.ai/docs/en/](https://catboost.ai/docs/en/)
This model gave us 92% accuracy for predicting genres. We tried to modify the original **Decision trees** model, but **CatBoost** was more effective and yielded the highest accuracy score.
Second best option was **XGBoost**, which is also gradient boosting algorithm based on **Decision Trees**

## Different types of machine learning models we tried:
 - Decision Trees - 67% accuracy
 - Recurrent Neural Network - 70% accuracy
 - Multinomial Logistical Regression - 72% accuracy
 - Neural Network - 88% accuracy
 - Random Forest - 88% accuracy
 - XGBoost - 90% accuracy
 - CatBoost - 92% accuracy


## Ethical Considerations
We are diligently looking to ensure the music copyrights are not violated.
Additionally we would like to mention this App is used as a student project.
No user data is collected.

## Data we used
**[GTZAN Music Genre Dataset](https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification)**  


## Future improvements
This project was done in 2 weeks and for future improvement, more genres could be added, different moods, similar lyrics, and playlists.
Better accuracy could be achieved. 






