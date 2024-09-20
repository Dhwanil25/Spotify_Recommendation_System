# Spotify Recommendation System 🎵
This project automates the creation of a personalized Spotify playlist by scraping Billboard Hot 100 songs for a specific date, adding them to a playlist, and recommending additional songs based on audio features. It integrates web scraping and Spotify API authentication to curate and enhance playlists based on user input.

# Features
- Scrapes the Billboard Hot 100 chart for a user-specified date.
- Authenticates with Spotify API to search for and add songs from the Billboard list.
- Automatically creates a private Spotify playlist with the selected songs.
- Extracts audio features (danceability, energy, tempo, valence) for the playlist songs.
- Uses K-Nearest Neighbors (KNN) to recommend similar songs based on their audio features.
- Adds the recommended songs to the created playlist.

# Requirements
- Python 3.x
- Spotipy (pip install spotipy)
- Beautiful Soup (pip install beautifulsoup4)
- Requests (pip install requests)
- Scikit-learn (pip install scikit-learn)
- Pandas (pip install pandas)

# Installation
1. Clone the Repository:
```bash
git clone https://github.com/Dhwanil25/Spotify_Recommendation_System.git
cd Spotify_Recommendation_System
```

2. Install the required libraries:
```bash
pip install -r requirements.txt
```

# Setup
3. Set up your Spotify Developer Account:

- Go to the [Spotify Developer Dashboard](https://developer.spotify.com/) and create a new application.
- Copy the Client ID and Client Secret to the script.

4. Update the CLIENT_ID and CLIENT_SECRET in the script with your credentials:

```python
CLIENT_ID = "your_client_id_here"
CLIENT_SECRET = "your_client_secret_here"
```

# Usage
1. Run the script:
```bash
python Spotify_Recommendation_System.py
```
2. Enter the date in the format YYYY-MM-DD when prompted. This date corresponds to the Billboard Hot 100 chart for that period:
```bash
Which era of music would you like to explore? Enter the date in the format YYYY-MM-DD to uncover the top songs from that time! 2022-01-01
```
3. The app will:

- Scrape the Billboard Hot 100 songs from the specified date.
- Create a private playlist in your Spotify account.
- Add the top songs and recommend similar tracks based on audio features.

# Technologies Used

- Python: Main programming language.
- Spotipy: For interacting with the Spotify API.
- BeautifulSoup: For web scraping Billboard's Hot 100.
- Scikit-learn: For using the K-Nearest Neighbors (KNN) algorithm to recommend similar songs.
- Pandas & NumPy: For data manipulation and analysis.

# License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

[Dhwanil Mori](https://github.com/Dhwanil25)
