# 🎥 Movie Recommendation System using Emotion

This project bridges the gap between Computer Vision and Content Discovery. By analyzing a user's facial expression, the system identifies their current emotion and recommends a curated list of movies from IMDb that match their mood.
🌟 Key Features

    Emotion Detection: Uses Deep Learning (DeepFace) to identify emotions like Joy, Sadness, Anger, or Surprise from photos.

    Real-time Scraping: Dynamically fetches the latest and top-rated movies from IMDb using BeautifulSoup; no static/outdated CSV datasets required.

    Intelligent Mapping: Automatically translates emotional states into movie genres (e.g., "Sad" ➡️ "Comedy" to lift spirits, or "Fear" ➡️ "Horror" for thrill-seekers).

    Robust Parsing: Employs RegEx to cleanly extract movie titles and metadata from complex HTML structures.

## 🛠️ Tech Stack

    Facial Analysis: DeepFace, OpenCV

    Web Scraping: BeautifulSoup4, Requests, lxml

    Data Handling: Python, re (Regular Expressions)

    Visualization: Matplotlib

## 🚀 How It Works

    Input: The user provides an image (via webcam or file upload).

    Analysis: The DeepFace library analyzes facial features to predict the dominant emotion.

    Fetching: The system selects the corresponding IMDb genre URL (e.g., https://www.imdb.com/search/title/?genres=drama).

    Output: The top 10-15 movie titles currently trending in that category are displayed to the user.

## 📂 Project Structure
Plaintext

├── app.ipynb               # Main logic: Scraping, Emotion Detection, and Logic
├── data/                   # (Optional) Cache for frequently accessed genres
├── uploads/                # Directory for user-input images
└── README.md               # Documentation

## 📈 Future Enhancements

    Streamlit Integration: Build a web-based UI for a more interactive user experience.

    Video Support: Enable real-time emotion tracking via live webcam feed.

    Multi-Platform Scraping: Expand beyond IMDb to include Rotten Tomatoes and Netflix trending lists.
