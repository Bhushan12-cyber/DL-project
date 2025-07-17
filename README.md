# Music Recommedation System
This is a Content-Based Music Recommendation System built using a CSV dataset of Spotify songs. The system recommends similar songs based on lyrics and audio features, using cosine similarity.

📁 Dataset
File: spotify_millsongdata.csv
Content: Lyrics and metadata for thousands of songs.

Columns: track, artist, text, and potentially processed features (e.g., TF-IDF of lyrics).

🔍 Features
Input a song title to get top 10 similar songs.

Uses cosine similarity on TF-IDF vectors of lyrics.

No need for external APIs like Spotipy – works offline.

⚙️ How It Works
Load Dataset

Reads the CSV file into a DataFrame.

Preprocessing

Converts lyrics to lowercase, removes stopwords and special characters.

Applies TF-IDF vectorization.

Similarity Calculation

Computes cosine similarity matrix.

Recommendation

User inputs a song name.

Returns top 10 lyrically similar songs based on vector similarity.

🛠 Technologies Used
Python (Jupyter Notebook)

pandas

scikit-learn (TF-IDF, cosine similarity)

NumPy
