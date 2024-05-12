
# Real Time Tamil Song Recommendation System

This project implements a real-time Tamil song recommendation system using data from Spotify's API. The system utilizes content-based and hybrid recommendation techniques to suggest songs similar to a given input song.

## Features

- **Fetching Data:** Utilizes Spotify's API to fetch data for tracks in a given playlist, including track name, artists, album name, release date, popularity, and audio features.
- **Content-Based Filtering:** Recommends songs based on similarity in audio features such as danceability, energy, key, loudness, mode, speechiness, acousticness, instrumentalness, liveness, valence, and tempo.
- **Hybrid Recommendations:** Enhances recommendations by combining content-based filtering with a weighted popularity score based on release date, providing a balance between similarity and popularity.

## Getting Started

1. **Obtain Spotify Client ID and Client Secret:** Replace `CLIENT_ID` and `CLIENT_SECRET` in the code with your own credentials obtained from the Spotify Developer Dashboard.
2. **Install Dependencies:** Ensure the required libraries are installed. You can do this by running `pip install spotipy`.
3. **Run the Code:** Execute the provided Jupyter Notebook or Python script to fetch data, preprocess it, and generate recommendations.

## Usage

1. **Input Song Name:** Specify the name of the input song for which recommendations are desired.
2. **Number of Recommendations:** Adjust the number of recommendations to be generated (default is 5).
3. **View Recommendations:** Check the hybrid recommended songs for the input song.

## Example

```python
input_song_name = "Valaiyosai"
recommendations = hybrid_recommendations(input_song_name, num_recommendations=5)
print(f"Hybrid recommended songs for '{input_song_name}':")
print(recommendations)
```

## Note

- Ensure your Spotify account has access to the playlist specified by `playlist_id`.
- The system currently supports Tamil songs; however, it can be extended to other languages or genres by modifying the playlist ID.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

