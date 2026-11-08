# Mixtape Metadata Assistant

A no-login, song-by-song helper for preparing Blogger entries for Mixtape.

## Features
- Enter a song title in English transliteration and choose its language.
- Open public searches for Google, YouTube, MSI, M3DB, MusicBrainz, Apple Music and Wikipedia.
- Check Apple's public iTunes Search API via JSONP for possible track/album results (no API key).
- Copy available Apple listing details into an editable form.
- Generate Blogger HTML using the metadata attributes expected by Mixtape: data-artist, data-music-director, data-lyricist, data-film, data-album, data-year, data-duration, data-audio and data-lyrics-url.
- Artwork is emitted as the first post image, matching Mixtape's current artwork parser.
- Copy or download generated HTML.

## Verification
This first version does not claim fully automatic film-credit discovery. Apple catalogue results can help identify a track and album, but do not reliably establish original film, music director or lyricist credits. Use source links to verify the correct version and edit fields. Search results are leads, not confirmed facts.

No login, API key or paid service is required. MusicBrainz opens as a public search page instead of being queried directly by browser code.

## GitHub Pages
Repository Settings > Pages > Deploy from a branch > main > /(root) > Save.

Expected URL: https://melvinvarghese.github.io/mixtape-metadata-assistant/
