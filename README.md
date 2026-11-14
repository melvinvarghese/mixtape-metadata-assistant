# Mixtape Metadata Assistant

A small web page for looking up a song and preparing the metadata block that [Mixtape](https://melvinvarghese.github.io/mixtape/) reads from a Blogger post.

Open it here: https://melvinvarghese.github.io/mixtape-metadata-assistant/

It is a single `index.html` file. There is no build step, no server, no account and no API key.

## Using it

1. Type the song title in English letters. Pick a language if you know it, and add a clue such as the film, a singer or the decade.
2. Press **Search sources**. The page does two things:
   - It looks up possible matches on Apple Music, JioSaavn and MusicBrainz and lists them as cards.
   - It builds search links for Spotify, YouTube, YouTube Music, JioSaavn, Gaana, Amazon Music, MusicBrainz, Apple Music and Google. MalayalaSangeetham (msidb.org) and M3DB are searched through Google.
3. Open the sources and check that they describe the right song and the right version. If a card looks right, press **Use these details** to copy its title, singer, album, year, duration and cover into the form.
4. Fill in what is still missing: music director, lyricist, lyrics page, audio link. None of the lookups return these.
5. Press **Generate Blogger HTML**, then copy it or download it, and paste it into Blogger's HTML view.

## What it generates

```html
<div class="mixtape-data" data-artist="..." data-music-director="..." data-album="..." data-year="..."></div>
<p><img src="..." alt="... cover"></p>
```

- Fields left empty are left out.
- The cover goes in as the first image of the post, because Mixtape takes artwork from there.
- For Apple results the cover link is changed to the 600 x 600 version.
- "Original Motion Picture Soundtrack" is dropped from album names.
- `utm_source=melvinvarghese.in` is added to the lyrics page link.
- Singers are separated by commas.

## Check the credits

A title match is not proof. Catalogue listings often have the wrong film, a remaster, or no music director or lyricist at all. Compare more than one source before you publish.

## Privacy

Whatever you type in the search box is sent to Apple (iTunes Search), JioSaavn, MusicBrainz and the search sites you open. Nothing is stored by this page.

JioSaavn results come from a community API (`saavn.dev`) that is not official and can be down. MusicBrainz can rate-limit requests. When a lookup fails, the page says so and the search links still work.
