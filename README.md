# Modeling Spotify User Behaviour

Welcome to my machine learning demo (in progress) using my own and an anonymous users' Spotify streaming and library data!

Goal:
- Predict song recommendations from user music preferences.

Current Status:
- [x] Created functions using the Spotify API for rapidly extracting audio features and genre information from a user's streaming history and library. 
- [x] Extracted audio features and genre information from 2 sets of streaming and library data.
- [x] Created functions for retreiving top 100 genres and songs in user streaming data.
- [x] Visualize when users listen to music during the day and year (add week as well)
- [x] Visualize if audio features of listened music changes throughout the day or week.
- [ ] Engineer a feature for liked vs disliked songs as a predictor. Examples:
   - Binary: listening time < 30s = dislike (0), otherwise 1
   - Continuous [0-1]: like index = listening time / track length
- [ ] Exploring genre latent space (audio features) with which we may be able to cluster music taste sentiments (THIS IS REALLY HARD SURPRISINGLY). So far:
  - [x] Principal component analysis on audio features to assess if music clusters by sentiment (Result: no obvious clusters)
  - [x] Principal component analysis on average genre audio features to assess if genres cluster by sentiment (Result: no obvious clusters)
  - [x] Group specific genres into their greater categories to reduce the number of genre classes
  - [ ] PCA on only a dozen selected genres
  - [x] Using random forest to explore audio features as genre predictors for a dozen or so overarching genres (this worked with roughly ~86% accuracy but I'm sure we can still do better)
- [ ] Modeling streaming tendencies for audiofeatures (what time of day do they listen to what kind of music? Can certain recommendations be tailored to specific times of day?)
- [ ] Predicting genre recommendations based on recent trends in audio features.

Given the project is a work in progress, much of the current work entails EDA. Ultimately, though the final goal is to perform advanced predictive modeling on user data so that we can predict prefered genres/audiofeatures using past streaming and library data.
