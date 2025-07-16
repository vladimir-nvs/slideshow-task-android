# Android Slideshow task

Your task is to develop a simple Android app that fetches and iterate over media files (images and videos) from NoviSign API. The app should display media items in a slideshow in a loop, with cross-fade transitions and display duration.

#### NoviSign api
1. Get playlist:

Inorder to get the  media files you need to fetch 'playlists' and extract the media files to display over the screen.
- The playlist might be empty.
- There can be more then one playlist.
- In your app you can use the following key:
```
https://test.onsignage.com/PlayerBackend/screen/playlistItems/e490b14d-987d-414f-a822-1e7703b37ce4
```
Response E.g:
```JSON
{
  "screenKey": "e490b14d-987d-414f-a822-1e7703b37ce4",
  "breakpointInterval": 0,
  "playlists": [
    {
      "channelTime": 0,
      "playlistItems": [
        "fileKey": "62ee6d0f-e058-43ce-907c-4133f12999c1.jpg"
      ]
    }
  ]
}
```

2. Get media files:

In order to recieve the media file you should call NoviSign's API with the relevant file key.
E.g:
```
https://test.onsignage.com/PlayerBackend/creative/get/2abbf8c1-396d-4fac-9a68-820c1abc6d96.png
```

### Bonus 
Check for playlist updates and display accordingly, without downloading unmodified items again.

##### What we anticipate to see in the  app:

1. Write the app with Java / Kotlin.
2. Using AI tools - big advantage. But you need to know what are changes implemented by AI tool.
3. Write unit tests
4. Use design patterns that allows flexible code structure, showing anticipation for evolution and new features 
5. Cut corners, but not to the point where the structure vanishes
6. Conventional coding style
7. README file and reasonable comments (where needed)
8. Upload project files to public GitHub repository

##### Question:
How would you have implement the Bonus question? (If you hadn't implemented it :) )
Answer the question in an answers.txt file

# Good luck!
