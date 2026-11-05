# NOCTURNE Music Player

A responsive music discovery player using Apple's iTunes Search API and LRCLIB lyrics API.

## Run it
1. Extract the ZIP.
2. Open the `aura-music-player` folder in VS Code.
3. Open `index.html` with Live Server, or simply open it in a modern browser.
4. Search for a song or artist.

No API keys or backend are required.

## Features
- Search up to 20 songs from iTunes (India storefront)
- 30-second audio previews when Apple provides a preview URL
- Album artwork and Apple Store link
- LRCLIB lyrics lookup; timestamped lyrics highlight in sync with preview playback
- Play/pause, previous/next, shuffle, repeat, seek and volume
- Favorites saved in browser LocalStorage
- Responsive dark glass-style UI

## Important API limitations
- iTunes `previewUrl` is generally a 30-second promotional preview, not full-song streaming.
- Apple requires promotional previews and artwork to be used to promote the corresponding iTunes content, with an appropriate Apple/iTunes store link and attribution. This UI includes an Apple link and “Previews provided courtesy of iTunes” attribution. Review Apple's current terms before public deployment.
- Lyrics availability and synchronization depend on LRCLIB's catalog. Some songs may have no lyrics or only plain lyrics.
- This is a front-end demo. It does not download or save audio.

## APIs
- iTunes Search: https://itunes.apple.com/search?term=QUERY&entity=song&limit=20&country=IN
- LRCLIB search: https://lrclib.net/api/search?q=TRACK%20ARTIST


## Visual update
The interface has been redesigned with a blue-violet glassmorphism layout inspired by the supplied reference: compact left playlist, large center artwork, right-side lyrics, and a bottom player dock.

demo""
https://music-player30.netlify.app/
