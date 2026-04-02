# Android Slideshow task

Develop a simple Android app that plays media in a slideshow.

The application should fetch playlist metadata and download images and videos from the server.
The media should be played in a loop with cross-fade transitions according to the duration in the metadata.
When playing offline, the app should be able to play the last downloaded playlist.
The app should periodically check for playlist changes (e.g. once per minute by default), download media in the background if needed, and play the modified playlist after a successful update.

#### User input

- The application should allow the user to enter a screen key.
- The user should be able to start and stop the playlist, and skip the current playback item.
- Screen key for testing: `7d47b6d7-8294-4b33-8887-066961d79993` — set it as the default on first launch

#### Server API

The API root URL is `https://test.onsignage.com/PlayerBackend/`

1. `screen/playlistItems` endpoint provides one or more playlists containing media item (creative) descriptor entries.

```text
screen/playlistItems/{screenKey}
```

- The playlist might be empty
- There can be more than one playlist
- Figure out which fields are useful and ignore response fields that are irrelevant for this task

2. `creative/get` endpoint serves a media file by `creativeKey`
```
creative/get/{creativeKey}
```

##### What we anticipate

- No clarification questions are expected:
  - Deriving *reasonable* details from the description is part of the assessment
  - If in doubt, make sane assumptions and document them
  - Let realistic app usage guide your decisions
- Java / Kotlin
- Use of AI tools is encouraged, provided that:
  - You should be able to explain the solution
  - You fully understand and stand behind any part of the generated code
  - You are able to quickly make changes to the generated code manually
- Efficient playlist and media updates
- Unit test coverage
- Use design patterns that allow flexible code structure, showing anticipation for evolution, new features, and configuration changes
- Cut corners (don't overcomplicate), but not to the point where the structure or architectural separation vanishes
- Conventional coding style
- README file, and reasonable code comments where appropriate

### Good luck!
