# MovieBuddy 🎬

**MovieBuddy** is a simple and interactive movie recommendation system built with Streamlit. It suggests 5 similar movies based on your favorite choice, using precomputed similarity scores and TMDB API for fetching posters.

## Features

- Select a movie from the dropdown
- Get top 5 recommended movies
- See posters of the suggested titles
- Built with Python, Streamlit, and TMDB API

## How to Run

1. Clone the repository and ensure all files (`movies.pkl`, `similarity.pkl`, `app.py`) are in the same directory.
2. Install the dependencies:
   ```bash
   pip install streamlit requests
