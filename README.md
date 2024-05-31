This project aims to quantify and visualize the lyrics of Taylor Swift's discography over the years to analyze the change in word choices using Genius API to download the artist’s entire discography, following the rules listed below. The lyrics are analyzed with pandas and NLTK, and visualized using WordClouds, matplotlib, and Plotly.

# Rules for Song Collection
Only certain songs from certain albums are included to simplify the song collection while still compiling the most data possible.
### Full studio albums are included.
* If there exists a deluxe edition, that is included instead of the standard edition.
* If multiple deluxe editions exist, the edition with the highest number of different songs is chosen.
* If the album was re-released as a Taylor’s Version* edition:
  * The original version is used; only vault songs from Taylor's Version are included.
### The following are NOT included:
* Songs that would cause duplicate lyrics:
  * remixes, acoustic, piano, live, or original demo versions
  * Taylor’s Version*
    * Only vault songs are included.
* EPs
* Songs originally released as singles or on soundtracks
* Anything written or spoken by the artist, such as: 
  * poems, voice memos, prologues, forewords, messages from artists, etc.
* Songs on which the artist is featured and songs the artist wrote for other artists.
* Covers and unreleased songs

# Files
* **genius_lyrics_collection** folder
  * Python code to extract lyrics of Swift’s songs from Genius API
  * 15 folders organized by album containing the song lyrics for each song as a .txt file
  * .csv file of every song containing data of the album, song name, and lyrics
* **p1_lyric_analysis** folder
  * Python code to perform word analysis
  * Python code to perform sentiment analysis
  * **graphs** folder
    * **word_analysis** folder
      * containing graphs creating during the word analysis
    * **sentiment_analysis** folder
      * containing graphs creating during the sentiment analysis
    
