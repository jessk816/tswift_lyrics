This project aims to quantify and visualize the lyrics of Taylor Swift's discography over the years to analyze the change in word choices using Genius API to download the artist’s entire discography, following the rules listed below. The lyrics are analyzed with pandas and NLTK, and visualized using WordClouds, matplotlib, and Plotly.

# Rules for Song Collection
To simplify the song collection while still compiling the most data possible, only certain songs from certain albums are included.
### Full studio albums are included.
* If there exists a deluxe edition, that is included instead of the standard edition.
* If multiple deluxe editions exist, the edition with the highest number of different songs is chosen.
* If the album was re-released as a Taylor’s Version* edition, only vault songs are included.
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
