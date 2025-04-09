# 🎵 Billboard Time Machine: Spotify Playlist Creator

Ever wondered what the top songs were on your birthday or any special day in history?  
**Billboard Time Machine** takes you back in time and automatically creates a **Spotify playlist** with the top 100 Billboard hits from that date!

🔗 **[Check out a sample playlist here](https://open.spotify.com/playlist/3mI5O7vgDv55rhopeRxwLV)**

---

## 🚀 Features

- ⏳ Scrapes Billboard Hot 100 for any date (YYYY-MM-DD format)
- 🎧 Automatically finds matching songs on Spotify
- 📝 Creates a **private playlist** on your Spotify account
- ⚡ Adds all the songs found to your new playlist

---

## 🛠️ Technologies Used

- `Python`
- `BeautifulSoup` & `requests` — for web scraping
- `Spotipy` (Spotify Web API) — for authentication and playlist creation

---

## 📦 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/billboard-spotify-playlist.git
   cd billboard-spotify-playlist
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up Spotify Developer credentials:**
   - Create an app on [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/)
   - Get your `Client ID`, `Client Secret`, and set the **Redirect URI** (e.g., `http://example.com`)

4. **Edit the script** (`main.py`) and replace:
   ```python
   client_id="YOUR_CLIENT_ID"
   client_secret="YOUR_CLIENT_SECRET"
   redirect_uri="YOUR_REDIRECT_URI"
   ```

---

## 🎬 Usage

1. Run the script:
   ```bash
   python main.py
   ```

2. Enter the date you want to travel back to:
   ```
   Which year do you want to travel to? Type the date in this format YYYY-MM-DD: 2001-06-15
   ```

3. Authorize the app via the browser pop-up.

4. Boom! 💥 Your playlist is ready in your Spotify account!

---

## 🧠 How It Works

- The script scrapes the Billboard Hot 100 chart from the provided date.
- It parses the song titles using `BeautifulSoup`.
- Using the Spotify Web API via `Spotipy`, it searches for each song.
- Found songs are added to a newly created private playlist on your Spotify.

---

## 📌 Notes

- Some older songs might not be available on Spotify and will be skipped.
- Make sure you have a valid Spotify account and you're logged in while authenticating.

---

## 🤝 Contributing

Feel free to fork the repo, raise issues, or open pull requests!  
Let's build something awesome together 🎧✨

---

