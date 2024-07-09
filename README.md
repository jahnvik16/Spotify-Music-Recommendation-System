# Spotify-Music-Recommendation-System

## Project Overview
This project implements a hybrid music recommendation system using Spotify's API. It combines content-based filtering with popularity-based recommendations to suggest similar songs based on a user's input.

## Features
- Fetches trending playlist data from Spotify
- Implements content-based filtering using audio features
- Incorporates popularity and recency into recommendations
- Provides hybrid recommendations based on song similarity and weighted popularity

## Technologies Used
- Python
- Pandas for data manipulation
- Spotipy for interacting with Spotify API
- Scikit-learn for machine learning operations (cosine similarity, MinMaxScaler)
- Requests for API calls
- Base64 for encoding client credentials

## Key Components

1. **Spotify API Authentication**
   - Utilizes client credentials flow for obtaining access token

2. **Data Retrieval**
   - Fetches track data from a specified Spotify playlist
   - Extracts detailed information including audio features, popularity, and release date

3. **Data Preprocessing**
   - Normalizes audio features using Min-Max scaling
   - Handles missing data

4. **Recommendation Algorithms**
   - Content-based filtering using cosine similarity of audio features
   - Popularity-based recommendations weighted by release date
   - Hybrid approach combining both methods

5. **User Interface**
   - Allows users to input a song name and receive recommendations

## How It Works
1. The system authenticates with Spotify API
2. It fetches and processes data from a trending playlist
3. When a user inputs a song, the system:
   - Finds similar songs based on audio features
   - Calculates a weighted popularity score considering release date
   - Combines these factors to produce hybrid recommendations

