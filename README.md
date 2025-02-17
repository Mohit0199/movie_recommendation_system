# Movie Recommendation System

This project implements a **Movie Recommendation System** using machine learning and content-based filtering. The recommendation engine suggests similar movies based on a selected movie using its metadata, such as genres, keywords, cast, and crew. The system leverages cosine similarity for recommending the most relevant movies.

## Project Overview

1. **Data Processing**:
   - The project starts with reading and merging movie data and credit data.
   - It processes the genres, keywords, cast, and crew columns by converting them into useful formats.
   - We use these features to create a unified tag for each movie by combining the movie's overview, genres, keywords, cast, and crew.

2. **Recommendation System**:
   - The recommendation engine is based on **Cosine Similarity** calculated on the tag data of each movie.
   - The system finds the top 5 most similar movies to the selected movie using the cosine similarity score.

3. **Streamlit App**:
   - The front-end application is built using **Streamlit** where users can select a movie and receive recommendations along with movie posters.
   - **TMDb API** is used to fetch movie posters dynamically based on the selected movie.

## Technologies Used

- **Python**: Programming language used.
- **Pandas**: For data manipulation.
- **NumPy**: For numerical operations.
- **Streamlit**: Framework for building the web app.
- **Scikit-learn**: Used for the cosine similarity calculations.
- **Requests**: To fetch movie posters from TMDb API.
- **TMDb API**: External API for movie data (like posters).
- **Pickle**: Used to serialize and save the data and model for later use.

## Features

- **Movie Selection**: Users can choose a movie from the dropdown list.
- **Recommendation Engine**: Based on the selected movie, the system provides 5 similar movie recommendations.
- **Movie Posters**: Display posters of the recommended movies using dynamic fetching from TMDb.
- **Real-time Recommendations**: The recommendation list and posters are updated in real time when the user selects a movie.
