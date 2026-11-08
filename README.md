# Mixtape Metadata Assistant

A browser-based helper for checking public song references and preparing Blogger-ready metadata for Mixtape.

**[Open the web app](https://melvinvarghese.github.io/mixtape-metadata-assistant/)**

## How to use it

1. Enter a song title in English transliteration. Choose a language and add an optional clue, such as a film, singer, or decade.
2. Select **Search sources**. Searches open for Google, YouTube, MalayalaSangeetham, M3DB, MusicBrainz, Apple Music, and Wikipedia. Possible Apple catalogue matches appear in the app when available.
3. Check that each result refers to the right song and version. You can copy available details from an Apple result, then edit or complete the fields yourself.
4. Add the credits and links you want to include, then select **Generate Blogger HTML**. Copy the result or download it as an HTML file, and paste it into Blogger’s HTML editor.

The editor includes fields for singers (separate multiple singers with commas), music director, lyricist, album or film, year, duration, lyrics URL, audio URL, and artwork URL. The generated Mixtape metadata block includes the available values; blank fields are left out. Artwork is added as the post’s first image so Mixtape can detect it.

## Check credits before publishing

Search results and Apple catalogue matches are clues, not verified credits. Catalogue listings may help identify a track or album, but they may not establish the original film, music director, or lyricist. Confirm the song version and credits against reliable sources before publishing.

## Access and data

The app requires no account, API key, or paid service. Searches open public source pages, and the app checks Apple’s public iTunes Search API for possible track matches. Search terms are sent to those services when you use them. The app has no server-side account or database.
