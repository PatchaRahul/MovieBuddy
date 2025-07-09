# MovieBuddy - Movie Recommendation System

## About the Project

MovieBuddy is a content-based movie recommendation system developed using Python and Streamlit. The system suggests movies that are similar to the one selected by the user. Instead of relying on user ratings or reviews, MovieBuddy focuses on the features of the movies themselves—such as title, genres, and overview—to find similarities and generate recommendations.

This project demonstrates how machine learning concepts can be applied in a real-world application, combining content filtering with a user-friendly web interface. It also integrates with the TMDB API to fetch and display high-quality movie posters, enhancing the overall user experience.

---

## Theory

The core idea behind MovieBuddy is **content-based filtering**, a recommendation method that compares items (in this case, movies) based on their content rather than user behavior.

Each movie is represented by a set of textual features (like plot summary and genres), which are converted into numerical vectors using vectorization techniques. These vectors capture the key traits of each movie.

To find similar movies, the system calculates the **cosine similarity** between the vectors. This measures how closely related two movies are in terms of their features. A higher cosine value means the movies are more similar. The system precomputes these similarity scores and uses them to provide quick recommendations.

---

## Features

- Allows users to select any movie from the list
- Recommends 5 similar movies instantly
- Displays movie posters using TMDB API
- Fast and lightweight user interface using Streamlit
- Content-based filtering model for personalized suggestions

---

## Technologies Used

- **Python** – for backend logic and ML model
- **Streamlit** – for building the web interface
- **Scikit-learn** – for calculating similarity
- **Pandas & NumPy** – for data manipulation
- **Pickle** – for loading pre-trained models
- **TMDB API** – to fetch real movie posters

---

## Functions and Logic

- `recommend(movie)`: Accepts a movie name and returns a list of 5 most similar movies and their poster URLs.
- `fetch_poster(movie_id)`: Uses the TMDB API to get the poster image of a given movie.
- Uses `cosine similarity` to measure closeness between movie vectors.
- Loads data from two `.pkl` files:
  - `movies.pkl` containing movie information
  - `similarity.pkl` containing similarity scores

---

## Why This Project?

- Recommender systems are widely used in platforms like Netflix, Amazon, and YouTube.
- This project provides hands-on experience with text processing, similarity algorithms, and interactive app development.
- It demonstrates how to apply machine learning without needing large datasets of user interactions.
- Integrates API usage, which is a valuable skill for any developer.

---

## File Structure

- `app.py`: Main application file with Streamlit code and logic
- `movies.pkl`: Serialized DataFrame containing movie titles and IDs
- `similarity.pkl`: Precomputed cosine similarity matrix
- `main.py`: Sample script (not essential to the app)
- `Projet Machine Learning.ipynb`: Optional notebook (can contain preprocessing or model-building steps)

# Output Preview
- On running the app, users will see a title and dropdown menu. After selecting a movie and clicking "Recommend," the app displays five recommended movies along with their images, arranged side by side.


